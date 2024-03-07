# WordPress Dockerized

## Overview

This project provides a Dockerized environment for running WordPress, MariaDB, and phpMyAdmin. Easily deploy a local development setup with Docker Compose, allowing you to efficiently manage your WordPress site and database.

## Features

- **WordPress:** Utilizes the official WordPress image with Apache server (version 6.2.2).
- **MariaDB:** Provides a MariaDB database with version 10.6.4-focal.
- **phpMyAdmin:** Includes phpMyAdmin for easy database management.
- **Docker Compose:** Simplifies the setup with a docker-compose.yml file.
- **Custom Networks:** Implements a custom bridge network for seamless communication between services.

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/wordpress-dockerized.git
   cd wordpress-dockerized
   ```
1. Create a ```.env``` file in the project root and set the following variables:

   ```bash
   MYSQL_ROOT_PASSWORD=your_root_password
   MYSQL_DATABASE=your_database_name
   MYSQL_USER=your_database_user
   MYSQL_PASSWORD=your_database_password
   ```
1. Run the Docker Compose:

   ```bash
   docker compose up
   ```

Access **WordPress** at ```http://localhost:8080``` and **phpMyAdmin** at ```http://localhost:8081```.
