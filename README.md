# Flask SQLAlchemy CRUD Application

This is a simple CRUD (Create, Read, Update, Delete) application built using Flask and SQLAlchemy. It provides an API to manage a collection of drinks.

## Setup

1. Make sure you have Python installed.
2. Install the required packages:

```bash
pip install Flask Flask-SQLAlchemy
```

Set up the MySQL database. Modify the SQLALCHEMY_DATABASE_URI in app.config to match your database configuration.

Create the database by running the following commands

1. Set up the MySQL database. Modify the SQLALCHEMY_DATABASE_URI in app.config to match your database configuration.

2. Create the database by running the following commands:

python
from your_script_name import db
db.create_all()
exit()

## Usage

-GET / - Returns "Hello, World!".

-GET /drinks - Returns a list of all drinks.

-GET /drinks/<id> - Returns details of a specific drink.

-POST /drinks - Adds a new drink. Requires a JSON payload with name and description.

-DELETE /drinks/<id> - Deletes a drink with the specified ID.

## Example Request

# Get all drinks

```bash
curl http://localhost:5000/drinks
```

# Get a specific drink

```bash
pip install Flask Flask-SQLAlchemy
```
# Delete a drink

```bash
curl -X DELETE http://localhost:5000/drinks/1
```

# Data Model

The application uses a simple Drink model with the following attributes:

-id (Integer, Primary Key) - Unique identifier for the drink.

-name (String, Unique, Not Null) - Name of the drink.

-description (String) - Description of the drink.
