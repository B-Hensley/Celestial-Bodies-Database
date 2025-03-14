# Celestial Bodies Database

This repository contains the code and schema for the Celestial Bodies Database project, completed as part of the FreeCodeCamp curriculum. The project involves creating a database to store information about celestial bodies in our solar system, including planets, moons, asteroids, and other relevant space objects.

## Features

- **Database Schema:** A well-defined schema to store celestial body information.
- **Data Entries:** Includes tables for planets, moons, asteroids, and other celestial objects.
- **Queries:** Basic SQL queries for managing and retrieving data related to celestial bodies.

## Technologies Used

- PostgreSQL for database management.
- SQL for querying and managing the database.

## Installation

To set up the project on your local machine, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/celestial-bodies-database.git
   ```
   
2. Navigate to the project directory:
   ```bash
   cd celestial-bodies-database
   ```
   
3. Create a PostgreSQL database:
   ```bash
   createdb celestial_bodies
   ```

4. Run the SQL script to create the necessary tables and insert sample data:
    ```bash
    psql -d celestial_bodies -f schema.sql
    ```

5. Connect to the PostgreSQL database:
    ```bash
    psql -d celestial_bodies
    ```

## Usage

You can query the database to retrieve information about celestial bodies. Here are some example queries:
  - Retrieve all planets in the solar system:
    ```sql
    SELECT * FROM planets;
    ```

  - Retrieve moons of a specific planet (e.g., Earth):
    ```sql
    SELECT * FROM moons WHERE planet_id = (SELECT id FROM planets WHERE name = 'Earth');
    ```

## License

This project is open source and available under the MIT License.
You can adjust the repository link and add any additional details if necessary!




