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
### Usage
 Visit http://localhost:5000 in your web browser to see the Flask application in action.
