# Nginx LocalStack Project

This project sets up an Nginx server that serves a "Hello World!" message and a LocalStack instance emulating AWS S3 using Docker Compose.

## Features

- Nginx server on port 8080 serving a static HTML page.
- LocalStack running on port 4566, emulating AWS services.
- Easy setup and usage with Docker Compose.

## Project Structure


- `docker-compose.yml`: Defines the LocalStack and Nginx containers.
- `nginx/default.conf`: Nginx configuration.
- `nginx/html/index.html`: The static HTML page served by Nginx.

## Getting Started

### Prerequisites

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/adiloc/musicals.git
   cd musicals

2. Run Docker Compose:
   ```bash
   docker-compose up

3. Access the Nginx "Hello World!" page in your browser:
   ```bash
   http://localhost:8080

4. Interact with LocalStack (e.g., creating an S3 bucket): 
   ```bash
   aws --endpoint-url=http://localhost:4566 s3 mb s3://my-local-bucket
 