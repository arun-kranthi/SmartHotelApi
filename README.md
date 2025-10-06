# SmartHotelApi

Minimal, ready-to-open ASP.NET Core Web API project skeleton for the Smart Hotel booking system.

## What's included
- ASP.NET Core Web API project (simple folder layout)
- Entities, DbContext (EF Core)
- Generic repository + Unit of Work
- Auth service with JWT (uses BCrypt for password hashing)
- Controllers: Auth, Hotels, Rooms, Bookings
- DTOs and AutoMapper mapping profile
- Sample `appsettings.json` and Program.cs

## How to run
1. Install .NET 7+ SDK.
2. Open the `SmartHotelApi.csproj` in `src/SmartHotel.Api` (or run from that folder).
3. Update connection string in `appsettings.json`.
4. Run migrations:
   ```bash
   dotnet tool install --global dotnet-ef
   dotnet ef migrations add InitialCreate
   dotnet ef database update
   ```
5. Start the API:
   ```bash
   dotnet run
   ```

A sample admin user is seeded with email `admin@smart.hotel` and password `Admin@123`.

