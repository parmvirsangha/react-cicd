# README

# React CI/CD Pipeline

[Deploy to Github Pages](https://github.com/parmvirsangha/react-cicd/actions/workflows/deploy.yml)

## Project Description

This project demos a complete CI/CD pipeline for a React app using Vite, Docker for local dev and Github Actions for automated deployment to Github Pages. It showcases DevOps practices such as containerization, automated workflows, and static site deployment

## Live Demo

[View the live demo](https://parmvirsangha.github.io/react-cicd/)

## Technology Stack

- React
- Vite
- Docker
- GitHub Actions
- GitHub Pages

## Local Development

### Prerequisites

- Docker and Docker Compose
- Git

### Setup and Run

1. Clone the repository

```bash

git clone https://github.com/parmvirsangha/react-cicd.git

cd react-cicd

```

2. Start the Docker development environment

```bash

docker-compose up

```

## Environment Variables

The application uses the following environment variables:

- `NODE_ENV` - Set to "development" for local development

## Deployment

This project is automatically deployed to GitHub Pages using GitHub Actions when changes are pushed to the main branch.

### Manual Deployment

If you want to deploy manually:

1. Build the application

```bash

npm run build

```

2. Deploy to GitHub Pages

```bash

npm run deploy

```

## GitHub Actions Workflow

The CI/CD pipeline includes the following steps:

1. Checkout code

2. Setup Node.js environment

3. Install dependencies

4. Build the application

5. Deploy to GitHub Pages

## Configuration Details

### GitHub Pages Configuration

- Base path: `/react-cicd/` (configured in vite.config.js)
- Homepage URL: `https://parmvirsangha.github.io/react-cicd`

### Docker Development Configuration

- Development server with hot reload
- Volume mounting for real-time code changes
- Port mapping from container to host
