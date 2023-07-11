This is a backend Node.js project called URL Shortener that allows you to shorten long links. It is built with Express.js, shortid, Mongoose, EJS, and dotenv dependencies.

Project Overview
The URL Shortener project provides a RESTful API for shortening long URLs. It generates a unique short code for each URL and maps it to the original long URL. When a user requests the short URL, they are redirected to the original long URL.

Installation
To install and run the URL Shortener project locally, follow these steps:

Clone the repository:
git clone https://github.com/your-favourphp/url-shortener.git

Navigate to the project directory:
cd url-shortener
Install the dependencies using npm
npm install
Create a .env file in the project's root directory and add the following environment variables:
PORT=2000


Modify the values according to your preferences or existing environment.

Start the server:
npm start
The server will run on http://localhost:2000.

Usage
Once the server is up and running, you can interact with the API using a tool like cURL, Postman, or any other HTTP client.
Shorten a URL
To shorten a long URL, send a POST request to the /api/url/shorten endpoint with the following JSON payload:
{
  "longUrl": "https://example.com/very/long/url"
}
The API will respond with a JSON object containing the shortened URL:
{
  "shortUrl": "http://localhost:2000/A9sGh3"
}
Redirect to Original URL
To redirect to the original long URL, simply visit the shortened URL provided by the API. For example:
http://localhost:2000/A9sGh3
You will be redirected to the original long URL associated with the provided short code.

Dependencies
The URL Shortener project utilizes the following dependencies:

Express.js: A fast and minimalist web application framework for Node.js.
shortid: A simple and dependency-free library for generating short, unique, non-sequential IDs.
Mongoose: An elegant MongoDB object modeling tool for Node.js.
EJS: A simple and flexible JavaScript templating engine that enables dynamic HTML rendering.
dotenv: A zero-dependency module for loading environment variables from a .env file into process.env.
Folder Structure
The project's folder structure is as follows:
url-shortener/
  │   ── db
          └──connect.js
  ├── models/
  │   └── shorturl.js
  ├── views/
  │   └── index.ejs
  ├── .env
  ├── .gitignore
  ├── server.js
  ├── package.json
  └── README.md
The config/ directory contains the database configuration file.
The models/ directory contains the Mongoose schema for the URL model.
The public/ directory contains the CSS file for the application's styling.
The views/ directory contains the EJS template for the index page.
The .env file stores environment variables.
The .gitignore file specifies which files and directories to exclude from version control.
The app.js file is the main entry point of the application.
The package.json file includes project metadata and lists the project's dependencies.
Contributing
Contributions to the URL Shortener project are welcome. If you find a bug or want to suggest an improvement, please create an issue or submit a pull request on the project's GitHub repository.

License
This project is licensed under the MIT License.






