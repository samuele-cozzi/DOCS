# Installation Identity Server Admin

[Skoruba.IdentityServer4.Admin](https://github.com/skoruba/IdentityServer4.Admin)

## Template

```
dotnet new -i Skoruba.IdentityServer4.Admin.Templates::1.0.0-beta7
```

## New Project
```
dotnet new skoruba.is4admin --name MyProject --title MyProject --adminrole MyRole --adminclientid MyClientId --adminclientsecret MyClientSecret
```

Modifica delle stringhe di connessione dei progetti e modificare il DB e lanciare i comandi dal progetto Admin:
```
dotnet ef database update -c AdminIdentityDbContext
dotnet ef database update -c AdminLogDbContext
dotnet ef database update -c IdentityServerConfigurationDbContext
dotnet ef database update -c IdentityServerPersistedGrantDbContext
```

## Endpoint
[Docs](http://docs.identityserver.io/en/latest/endpoints/discovery.html)

```
/connect/authorization
/connect/token
```
