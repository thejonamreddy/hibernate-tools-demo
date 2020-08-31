# Hibernate Tools Demo

This project was generated with [Spring Initializr](https://start.spring.io).

## Reference

https://jonamlabs.com/how-to-use-hibernate-tools-maven-plugin-to-generate-jpa-entities-from-an-existing-database/

## Setup

1. Ensure [Docker](https://www.docker.com/) is installed and running on your machine
2. Run `docker-compose up -d` to start the MySQL instance in the background
3. The above MySQL instance will be initialized with the `initdb.sql`
4. Run `mvn hibernate-tools:hbm2java` to convert database tables into JPA entities
5. The JPA entities will be generated to the `${project.basedir}/src/main/java/com/jonamlabs/hibernatetoolsdemo/entity` folder