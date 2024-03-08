<h1>Dockerized Flask App</h1>



## About The Project

This project is a Dockerized Flask application designed to simplify deployment and ensure consistency across different environments. It's ideal for development and production setups, providing an easy-to-use template for containerizing Python web applications.

### Features

- Fully Dockerized environment for Flask.
- Simple to scale and deploy.
- Includes a sample Flask application to get started quickly.
- Utilizes best practices for Docker and Flask development.

## Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

- Docker
- Docker Compose (optional)

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/SanidhyaShrivastava/Dockerize_Flask_App.git
2. Build the Docker container
   ```sh
   docker build -t flask-app .
3. Run the Docker container
   ```sh
   docker run -d -p 5000:5000 flask-app

### Database Setup and Migrations
1. Run a container using the `notesapp` image and mount the migrations directory:
   ```sh
   docker run --rm -it --network notes -v /home/cloud_user/notes/migrations:/app/notes/migrations notesapp:0.1 bash
2. Once connected to the container, initialize the database with Flask-Migrate:
   ```sh
   flask db init
3. Check the migrations folder to ensure the `init` command has created the necessary files:
   ```sh
   ls -l migrations
4. Create the migration scripts needed to set up the database schema:
   ```sh
   flask db migrate
5. Apply the migrations to the database:
   ```sh
   flask db upgrade


### Usage
 Visit http://localhost:5000 in your web browser to see the Flask application in action.
