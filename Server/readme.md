### should be added libs 
Microsoft.EntityFrameworkCore.Design
Microsoft.EntityFrameworkCore
Microsoft.EntityFrameworkCore.Sqlite

### 1 step. install entity framework tool
dotnet tool install --global dotnet-ef --version 6.0.0
if an error occurs:
> dotnet new tool-manifest
> dotnet restore --interactive
> 
### 2 step. 
cd Server
### 3 step. first migration
dotnet-ef migrations add InitialMigration -o "Data/Migrations"

migration class is specified witch changes applied to database

### generate database
dotnet ef database update
