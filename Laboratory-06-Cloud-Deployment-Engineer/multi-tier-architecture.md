# Two-Tier Architecture

## What Is Two-Tier Architecture?

Two-tier architecture is a system architecture in which an application is divided into two main parts or tiers. The first tier handles the application or user-facing functions, while the second tier handles the database and data storage.

In this laboratory activity, the two tiers are represented by the Nextcloud application and the MariaDB database.

## Web/Application Tier

The Web/Application Tier contains the Nextcloud application. It is responsible for providing the web interface and handling application functions.

In the Docker Compose configuration, the application tier is represented by the `app` service:

    app:
      image: nextcloud
      ports:
        - 8080:80

The Nextcloud application is accessed through port 8080 on the host machine.

## Database Tier

The Database Tier contains the MariaDB database. It is responsible for storing the data used by the Nextcloud application.

In the Docker Compose configuration, the database tier is represented by the `database` service:

    database:
      image: mariadb:10.6

The MariaDB container stores and manages the database used by Nextcloud.

## Why Separate the Application and Database?

The application and database are separated into different containers so that each component has its own role. The Nextcloud container focuses on running the application, while the MariaDB container focuses on storing and managing data.

This separation makes the system easier to organize and manage. Each service can be configured and maintained independently while still communicating with the other service.

    (Database Container)

The Nextcloud application communicates with the MariaDB database through the database service defined in the Docker Compose configuration.
