# SQL Server

Spins up a SQL Server database along with the [Adminer](https://www.adminer.org/) portal.


## Run

Run `docker-compose up` to spin up the resources

Go to `localhost:8080` to access the Adminer portal and enter the following values

| Property | Value         |
| -------- | ------------- |
| System   | SQL Server    |
| Server   | sql-server-db |
| Username | SA            |
| Password | Admin12#      |


You can also SSH into the SQL Server container to run SQL commands
```
docker exec -it <CONTAINER_ID> bash
/opt/mssql-tools/bin/sqlcmd -S localhost -U SA -P "Admin12#"
```
