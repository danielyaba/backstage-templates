# ${{ values.name }} NodeJS application

## Overview

This is the git repository for ${{ values.name }} NodeJS application
It includes a basic project structure, sample configuration files, and a predefined GitHub Actions workflow for continuous integration and deployment.

## Project Structure 
The project follows a standard Node.js application structure:  
```
.
├── Dockerfile
├── README.md
├── catalog-info.yaml
├── deployment
│   ├── Chart.yaml
│   └── values.yaml
├── package.json
└── src
    └── index.js
```

- **Dockerfile**: A Dockerfile for containerizing the application.
- **README.md**: This readme file.
- **catalog-info.yaml**: Backstage catalog information for registering the component.
- **package.json**: The project configuration file for npm.
- **src/**: The directory of the application code.
- **deployment/**: The directory for Helm-Chart used by ArgoCD for continues deployment.
- **.github/workflows/build-and-push.yaml**: A GitHub Actions workflow for building and pushing Docker images.


## Getting Started

### Prerequisites

Ensure you have the following installed:

- Node.js (v18 or higher)
- npm (v7 or higher)
- Docker

### Installation

1. Clone the repository:
```
git clone https://github.com/your-username/my-first-node-app
cd my-first-node-app
```

2. Install dependencies:
```
npm install
```

3. Running the application:
```
npm start
```