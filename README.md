# Caddy Docker Setup

This repository contains the necessary files to set up a Docker container running Caddy web server. The setup includes:

1. A Dockerfile that pulls a Caddy image, copies a test HTML file and a Caddyfile.
2. A Caddyfile that configures Caddy to run on port 8080 and uses `/home` as the root directory for files.
3. A test HTML file that displays static content.

## Files

- `Dockerfile`: Defines the Docker image setup.
- `Caddyfile`: Configures Caddy server settings.
- `index.html`: Test HTML file with static content.

## Instructions

### 1. Clone the Repository

```sh
git clone https://github.com/cyse7125-su24-team15/static-site
cd static-site
```

### 2. Dockerfile

The `Dockerfile` is used to create a Docker image using the caddy image

### 3. Caddyfile

The `Caddyfile` configures Caddy to run on port 8080 and serves files from `/home`:

### 4. index.html

The `index.html` is a simple HTML file to serve test content:

### 5. Build and Run the Container

To build and run the Docker container, follow these steps:

#### Build the Docker Image

```sh
docker build -t caddy-test .
```

#### Run the Docker Container

```sh
docker run -d -p 8080:8080 caddy-test
```

### 6. Access the Test Page

Open a web browser and go to `http://localhost:8080` to see the test page.
