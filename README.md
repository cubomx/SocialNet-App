# Setup Environment

## VS Code
Install the following extensions:
- [C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp)
- [C# Extensions](https://marketplace.visualstudio.com/items?itemName=kreativ-software.csharpextensions)
- [NuGet Gallery](https://marketplace.visualstudio.com/items?itemName=patcx.vscode-nuget-gallery)
- [SQLite](https://marketplace.visualstudio.com/items?itemName=alexcvzz.vscode-sqlite)

## Install dependencies
Install [Entity Framework Core Tools](https://www.nuget.org/packages/dotnet-ef/) for the .Net CLI:
```csharp
dotnet tool install --global dotnet-ef --version <Version>
```

Install the .NET HTTP REPL CLI to make HTTP requests:
```csharp
dotnet tool install -g Microsoft.dotnet-httprepl
```

## Project
Create solution:
```csharp
dotnet new sln
```

Create project
```csharp
dotnet new <Template>
```

Link project to solution
```csharp
dotnet sln add <ProjectSource>
```

Create certificate
```csharp
dotnet dev-certs https --trust
```

## DB Setup
Install the following packages in the NuGet Gallery:
- **Microsoft.EntityFrameworkCore.Sqlite** (or )


Create the database schema
```csharp
dotnet ef migrations add <Name> -o <DataFolder>/Migrations
```

Create or modify 
```csharp
dotnet ef database update
```
