
# Full-Stack FastAPI and React Template

Welcome to the Full-Stack FastAPI and React template repository. This repository serves as a demo application for interns, showcasing how to set up and run a full-stack application with a FastAPI backend and a ReactJS frontend using ChakraUI.

## Prerequisites

Before you begin, ensure you have installed the following:

- Python (>= 3.8)
- Node.js (>= 14.x)
- Docker (optional for Docker deployment)

## Manual Deployment

### Running the backend locally

1. Clone the repository to your local machine.

    ```sh
    git clone <repository_url>
    ```

2. Navigate to the `backend` directory and install the Python dependencies
    ```sh
    cd backend
    poetry install
    ```

3. Update the configuration file in the `.env` with your data

4. Set up the database with the necessary tables
    ```sh
    poetry run bash ./prestart.sh
    ```

5. Run the backend server
    ```
    poetry run uvicorn app.main:app --reload
    ```

### Running the frontend locally

1. Clone the repository to your local machine.

    ```sh
    cd frontend
    ```

2. Navigate to the `frontend` directory and install the Frontend dependencies
    ```sh
    npm install
    ```

3. Update the configuration file in the `.env` with your data

4. Run the backend server
    ```sh
    npm run dev
    ```

## Docker Deployment

### Using Docker Compose

1. Install Docker Compose if you haven't already.
2. Run `docker-compose up -d` to start both the backend and frontend services.

## Project Structure

The repository is organized into two main directories:

- **frontend**: Contains the ReactJS application.
- **backend**: Contains the FastAPI application and PostgreSQL database integration.

Each directory has its own README file with detailed instructions specific to that part of the application.
- [Frontend README](./frontend/README.md)
- [Backend README](./backend/README.md)

