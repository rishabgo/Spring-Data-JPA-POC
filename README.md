# Spring-Data-JPA-POC
An example project showing how to configure multiple datasource in spring boot to work with spring-data-jpa.

Separate @Configuration files are created for each datasource (customer, product). Mysql and Postgres databases are used in the example, but this setup can be used for any database.

# Starting Databases
docker run -p 3306:3306 --name my-mysql -e MYSQL_ROOT_PASSWORD=password -d mysql:latest

docker run --name some-postgres -e POSTGRES_PASSWORD=password -p 5432:5432 -d postgres:latest
