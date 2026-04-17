# SistemaAdministracion - API
Proyecto inicial: API .NET Core para sistema administrativo contable.

Caracteristicas incluidas en este commit:
- API .NET 7 (esqueleto)
- PostgreSQL (docker-compose)
- EF Core con Npgsql
- JWT Authentication
- Módulos: Auth (login/registro) y Sales (facturas)

Instrucciones rápidas:
1. Copiar `appsettings.json` y ajustar la cadena de conexión y JWT Secret o usar variables de entorno.
2. Levantar Postgres: `docker-compose up -d`
3. Aplicar migraciones: `dotnet ef database update --project src/SistemaAdmin.Api`
4. Ejecutar: `dotnet run --project src/SistemaAdmin.Api`

Notas:
- Este es un esqueleto inicial para trabajar por módulos. Implementaciones de negocio se deben ampliar según requisitos.