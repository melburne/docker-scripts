# MySQL

Spins up a MySQL database along with the [Adminer](https://www.adminer.org/) portal.


## Run

Run `docker-compose up` to spin up the resources

Go to `localhost:8080` to access the Adminer portal and enter the following values

| Property | Value         |
| -------- | ------------- |
| System   | MySQL         |
| Server   | mysql-db      |
| Username | root          |
| Password | root          |


You can also SSH into the MySQL container to run SQL commands
```
docker exec -it <CONTAINER_ID> bash
mysql -u root -proot
```
