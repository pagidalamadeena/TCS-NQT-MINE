**Entity Framework Core 8.0:-**





&#x20; 1. Overview of EF Core 8 and .NET 8 Integration



&#x20; What is ORM (Object‑Relational Mapping)?



\*   Technique to map C# objects to database tables

\*   Eliminates manual SQL for CRUD

\*   Converts rows ↔ objects automatically

\*   Improves productivity and maintainability



&#x20;



&#x20; EF Core vs EF Framework (EF 6) – Key Differences



\*   EF Core:

&#x20;   \*   Lightweight and cross‑platform

&#x20;   \*   High performance

&#x20;   \*   Works with .NET 8

&#x20;   \*   Supports modern features (async, compiled queries)

\*   EF Framework:

&#x20;   \*   Windows‑only

&#x20;   \*   Heavier and older

&#x20;   \*   Limited performance optimizations



&#x20;



&#x20; New Features in EF Core 8



\*   Improved query translation and performance

\*   Better JSON column support

\*   Enhanced bulk operations

\*   Optimized compiled queries

\*   Improved migrations and scaffolding

\*   Better support for .NET 8 async patterns



&#x20;



&#x20; 2. Setting up EF Core in a .NET 8 Project



&#x20; Installing EF Core Packages via NuGet



\*   `Microsoft.EntityFrameworkCore`

\*   `Microsoft.EntityFrameworkCore.SqlServer`

\*   `Microsoft.EntityFrameworkCore.Tools`

\*   Installed using NuGet Package Manager or CLI



&#x20;



&#x20; Configuring DbContext



\*   DbContext represents a database session

\*   Contains DbSet<TEntity> properties

\*   Configured using `OnConfiguring` or `Program.cs`



&#x20;



&#x20; Connecting to SQL Server



\*   Uses connection string

\*   Configured with `UseSqlServer()`

\*   Stored in `appsettings.json`



&#x20;



&#x20; Basic EF Core CLI Commands



\*   `Add-Migration MigrationName`

\*   `Update-Database`

\*   `Remove-Migration`

\*   Used to manage database schema changes



&#x20;



&#x20; 3. Creating a Simple Database Model



&#x20; Defining Entities and Relationships



\*   Entity = C# class mapped to a table

\*   Properties map to table columns

\*   Relationships defined using navigation properties



&#x20;



&#x20; Primary Keys, Foreign Keys, Navigation Properties



\*   Primary Key:

&#x20;   \*   Uniquely identifies a record

&#x20;   \*   Usually `Id`

\*   Foreign Key:

&#x20;   \*   References another table’s primary key

\*   Navigation Property:

&#x20;   \*   Enables object navigation between entities



&#x20;



&#x20; Code‑First Approach Overview



\*   Database generated from C# classes

\*   Changes tracked via migrations

\*   No manual DB creation required



&#x20;



&#x20; 4. Performing Basic CRUD Operations



&#x20; Inserting Records (AddAsync)



\*   `AddAsync()` adds entity to context

\*   `SaveChangesAsync()` persists data

\*   Entity tracked by DbContext



&#x20;



&#x20; Retrieving Data



\*   `Find()` → Fetch by primary key

\*   `FirstOrDefault()` → First matching record

\*   `ToListAsync()` → Retrieves all records



&#x20;



&#x20; Updating Records and Tracking Changes



\*   EF Core tracks entity state

\*   Changes detected automatically

\*   `SaveChangesAsync()` updates DB



&#x20;



&#x20; Deleting Records



\*   `Remove()` → Delete single entity

\*   `RemoveRange()` → Delete multiple entities

\*   Changes saved using `SaveChangesAsync()`



&#x20;



&#x20; 5. LINQ Queries in EF Core 8



&#x20; Writing Queries



\*   `Where()` → Filtering

\*   `Select()` → Projection

\*   `OrderBy()` / `OrderByDescending()` → Sorting



&#x20;



&#x20; Projection into DTOs



\*   DTO = Data Transfer Object

\*   Improves performance

\*   Transfers only required fields



&#x20;



&#x20; Filtering and Aggregating Data



\*   Filtering: `Where()`

\*   Aggregation: `Count()`, `Sum()`, `Average()`, `GroupBy()`



&#x20;



&#x20; Asynchronous Queries



\*   `ToListAsync()`

\*   `FirstOrDefaultAsync()`

\*   Improves scalability and responsiveness



&#x20;



&#x20; 6. EF Core Migrations and Database Updates



&#x20; Adding, Removing, and Updating Migrations



\*   `Add-Migration` → Create migration

\*   `Remove-Migration` → Undo last migration

\*   `Update-Database` → Apply migration



&#x20;



&#x20; Seeding Data during Migrations



\*   Insert initial/static data

\*   Defined using `HasData()`

\*   Useful for default values



&#x20;



&#x20; Managing Database Schema Changes



\*   Schema changes tracked via migrations

\*   Version control friendly

\*   Supports rollback



&#x20;



&#x20; 7. Handling Relationships and Data Loading



&#x20; Eager, Lazy, and Explicit Loading



\*   Eager Loading:

&#x20;   \*   Uses `Include()`

&#x20;   \*   Loads related data immediately

\*   Lazy Loading:

&#x20;   \*   Loads data on demand

&#x20;   \*   Requires proxies

\*   Explicit Loading:

&#x20;   \*   Manually loads related data



&#x20;



&#x20; Configuring Relationships



\*   One‑to‑One

\*   One‑to‑Many

\*   Many‑to‑Many

\*   Configured using navigation properties and Fluent API



&#x20;



&#x20; Navigating Circular References



\*   Occur in bidirectional relationships

\*   Can cause serialization issues

\*   Handled using DTOs or JSON settings



&#x20;



&#x20; 8. Performance Optimizations and Best Practices



&#x20; Query Tracking and Caching



\*   `AsNoTracking()`:

&#x20;   \*   Disables change tracking

&#x20;   \*   Improves read performance

\*   Useful for read‑only queries



&#x20;



&#x20; Batch Processing and Bulk Operations



\*   Reduces database round‑trips

\*   Improves performance for large data operations

\*   Supported better in EF Core 8



&#x20;



&#x20; Handling Concurrency



\*   Uses `RowVersion` (timestamp column)

\*   Detects conflicting updates

\*   Prevents data loss



&#x20;



&#x20; Compiled Queries



\*   Precompiled LINQ queries

\*   Improves repeated query performance

\*   Reduces query translation cost



&#x20;

