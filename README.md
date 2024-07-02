# 🥕 Restaurant API

## Overview

Welcome to the Restaurant API This API allows you to manage your virtual tavern seamlessly with AdonisJS 5 and TypeScript, featuring robust table management functionalities. For development, we utilize SQLite3, while MySQL is used for production. Additionally, the API is designed with Test-Driven Development (TDD) options to ensure reliable and maintainable code.

## Features

- **Table Management:** Manage tables, reservations, and seating arrangements effortlessly.
- **TypeScript:** Enjoy type safety and modern JavaScript features.
- **AdonisJS 5:** Leverage the power of AdonisJS, a fully-featured Node.js framework.
- **SQLite3 for Development:** Lightweight and easy-to-use database for local development.
- **MySQL for Production:** Reliable and scalable database solution for production.
- **TDD:** Implement Test-Driven Development for robust testing capabilities.

## Tech Stack

- **Languages:** TypeScript
- **Framework:** AdonisJS 5
- **Databases:** SQLite3 (development), MySQL (production)
- **Testing:** TDD

## Getting Started

### Prerequisites

- Node.js
- npm or yarn
- SQLite3 (for development)
- MySQL (for production)

### Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/malldonado/api-restaurante.git
    cd api-restaurante/roleplay-api
    ```

2. **Install dependencies:**

    ```bash
    npm install
    # or
    yarn install
    ```

3. **Set up the environment variables:**

    Create a `.env` file in the root directory and add the following variables:

    ```env
    NODE_ENV=development
    APP_KEY=your_app_key
    DB_CONNECTION=sqlite
    SQLITE_FILENAME=./db.sqlite3
    MYSQL_HOST=127.0.0.1
    MYSQL_PORT=3306
    MYSQL_USER=root
    MYSQL_PASSWORD=your_mysql_password
    MYSQL_DB_NAME=restaurant
    ```

4. **Run migrations:**

    ```bash
    node ace migration:run
    ```

### Running the Development Server

Start the AdonisJS development server:

```bash
npm run dev
# or
yarn dev
```

## Starting the Server

The server will start on http://localhost:3333.

## Testing

To run tests, use the following command:

```bash
npm run test
# or
yarn test
```

## API Endpoints

### Tables

- `GET /tables`: Retrieve a list of all tables.
- `POST /tables`: Create a new table.
- `GET /tables/:id`: Retrieve a single table by ID.
- `PUT /tables/:id`: Update a table by ID.
- `DELETE /tables/:id`: Delete a table by ID.

## Database Configuration

### Development

For development, we use SQLite3. The configuration is set in the `.env` file:

```dotenv
DB_CONNECTION=sqlite
SQLITE_FILENAME=./db.sqlite3
```

## Production

For production, we use MySQL. Update the `.env` file with your MySQL credentials:

```env
DB_CONNECTION=mysql
MYSQL_HOST=127.0.0.1
MYSQL_PORT=3306
MYSQL_USER=root
MYSQL_PASSWORD=your_mysql_password
MYSQL_DB_NAME=restaurant
```

# Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-foo`).
3. Commit your changes (`git commit -am 'Add foo feature'`).
4. Push to the branch (`git push origin feature-foo`).
5. Create a new Pull Request.

# License

This project is licensed under the MIT License. See the LICENSE file for details.

# Acknowledgements

- AdonisJS
- TypeScript
- SQLite
- MySQL

This README.md provides a comprehensive overview of the API, including instructions for installation, configuration, execution, and testing, as well as details about the functionalities and the technological stack used in the project.
