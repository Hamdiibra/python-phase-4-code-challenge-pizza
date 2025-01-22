## Pizza Restaurant API

# Overview:

This API allows users to manage restaurants, pizzas, and their relationships through the RestaurantPizza model. The functionality includes retrieving restaurant and pizza data, adding pizzas to restaurants, and managing these resources with appropriate validations and cascading deletions.

# Features:

1. CRUD operations for restaurants and pizzas.

2. Many-to-many relationship between restaurants and pizzas through the RestaurantPizza model.

3. Validations for price range on RestaurantPizza.

4. JSON serialization with customizable fields to control recursion depth.

# Setup

Follow these instructions to set up and run the project:

1. Prerequisites

2. Python 3.8+

3. Flask and its extensions (Flask-Migrate, Flask-RESTful, SQLAlchemy)


# Installation

- Clone the repository and navigate to the project directory.

- Install Python dependencies:
``` bash
pipenv install
pipenv shell
```

- Install frontend dependencies (optional):

``` bash npm install --prefix client```

- Database Setup
```bash
export FLASK_APP=server/app.py
flask db init
flask db migrate -m 'Initial migration'
flask db upgrade head
```

- Seed the database:

```bash 
python server/seed.py
```

- Running the Application

1. Start the Flask API server:

```bash
 python server/app.py
```

- (Optional) Start the React frontend:

```bash 
npm start --prefix client
```


# Testing

1. To test the API endpoints, you can use tools like Postman, cURL, or the provided React frontend.

2. Seed the database with sample data using python server/seed.py.

Enjoy managing your pizza restaurants with this API!

