# MS SQL

Docker Pull

```shell
docker pull mcr.microsoft.com/mssql/server
```

Docker Run

```shell
docker run -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=Openjob_01" -p 1433:1433 -d mcr.microsoft.com/mssql/server:2019-GDR1-ubuntu-16.04
```
