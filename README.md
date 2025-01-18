# Docker Demo Project

A simple web application demonstrating Docker container usage with Nginx. The project includes two versions:
1. A basic "Hello" page
2. An enhanced version with custom content and a login system

## Prerequisites

- Docker installed and running on your machine
- Git Bash (recommended for Windows users) or Unix-like terminal

## Project Structure

```
demoDocker/
├── app/
│   ├── index.html
│   ├── main.css
│   ├── main.js
│   └── content.html
├── compose.yaml
└── up.sh
```

## Setup and Installation

1. Clone this repository
2. Navigate to the project directory:
   ```bash
   cd demoDocker
   ```
3. Start the Docker container:
   ```bash
   source up.sh
   # Or alternatively:
   . up.sh
   ```
4. Access the application at `http://localhost:81`

## Features

### Version 1: Basic Hello Page
- Simple "Hello" message
- CSS styling with aqua background
- JavaScript alert on page load

### Version 2: Enhanced Content with Login
- Login system with hardcoded credentials (for demonstration purposes only)
- Custom content page
- Basic authentication before accessing main content

## Technical Details

- Uses Nginx web server image
- Port mapping: 81:80
- Volume mounting for static files
- Docker Compose for container orchestration

## Security Note

The login system in this demo uses hardcoded credentials for educational purposes only. In a production environment, proper authentication and security measures should be implemented.

## Docker Commands

Check Docker installation:
```bash
docker --version
```

Check running containers:
```bash
docker ps
```
