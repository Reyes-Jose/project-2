# Restaurant Reviews 

## Add reviews for your favorite restaurants!

Everybody loves food and looking at reviews before going to restaurants is a huge part of foodie culture. Our app provides a brief list, introduction of restaurants, and review by users. 
It pulls information from (our RESTful API?) and provides reviews of users that have been to the restaurant before. Additionally, it contains a login page and profile page that allows users to create their own reviews in real time. The app has a feature to save the reviews to the profile page as well as the main page containing the restaurants. It also let users to remove previous reviews from the list. 

## User Story

I want to access and write restaurant reviews based on the restaurant name. So that I can easily see if pets are allowed and if the environment and food of the restaurant are what I am looking for.

As a user, I want to add reviews with my experience of those restaurants. Those reviews are then saved in my profile page and I am able to access my previous reviews with the ability to delete them.

## Technologies used

Node.js and Express.js to create a RESTful API. Handlebars.js as the template engine and display. MySQL and the Sequelize ORM for the database. Incorporation of GET and POST routes for retrieving and adding new data. Usage of Bulma for styling. 

## Application Links

- [Deployed App on Heroku](https://restreviews-app.herokuapp.com/)
- [GitHub Repository](https://github.com/Reyes-Jose/project-2)

## Screenshot

![Screenshot of App](./assets/example.png)

## Running the App Locally

For development, the app can be hosted locally.

First, clone the repo. Then:

- Install the Node dependencies:

    ```bash
    npm install
    ```

- Copy the `dotenv` example file (`.env.example`) to a new `.env` file
  - (The `.env` file is included in the `.gitignore`, so no need to worry about committing your local credentials)

  ```bash
  cp .env.example .env
  ```

- Populate the `.env` file with your MySQL credentials:

    ```toml
    DB_NAME='restreview_db'
    DB_USER='<username_goes_here>'
    DB_PASSWORD='<password_goes_here>'
    ```

- Source the MySQl schema:

    ```bash
    mysql -u root -p
    ```

    ```sql
    SOURCE ./db/schema.sql;
    exit;
    ```

- Seed the database locally:

    ```bash
    npm run seed
    ```

- Then start the App:

    ```bash
    npm start
    ```

## Contributors

Made by Kristina Litunovskaia, Maryam Muska, Ryan Whitmore, Jose Reyes, and William Huang.
