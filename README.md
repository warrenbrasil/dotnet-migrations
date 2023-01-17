# Warren - .NET Migrations :cd:

This action is responsible for applying .NET migrations to a database

## Inputs

### `project-path`

**Required**: The path for the project that holds the migrations folder

### `startup-project-path`

**Required**: The startup project of the application

### `context`

**Required**: The DbContext class name

### `connection`

**Required**: The connection string for the database to apply migrations

## Usage

```yml
- name: Warren - Configure .NET SDK
  uses: warrenbrasil/dotnet-migrations@v2
  with:
    project-path: ./src/FooProject
    startup-project-path: ./src/FooProject.API
    context: FooDbContext
    connection: <CONNECTION_STRING_GOES_HERE>
```
