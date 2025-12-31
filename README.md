# fullstack_developer_capstone

## Project Description
This is a full-stack developer capstone project that demonstrates a complete web application with a Django backend, microservices architecture, and a React frontend. The application appears to be a car dealership management system with features for handling dealerships, inventory, reviews, and sentiment analysis.

## Features
- **Backend**: Django-based server with REST APIs for managing dealership data, inventory, and reviews
- **Microservices**: Sentiment analysis service for processing reviews
- **Database**: Node.js-based microservices for dealership, inventory, and review management
- **Frontend**: React application for user interface
- **Deployment**: Docker containerization with docker-compose for easy deployment

## Tech Stack
- **Backend**: Django, Python
- **Microservices**: Node.js, Python (for sentiment analysis)
- **Database**: JSON-based data storage (car_records.json, dealerships.json, reviews.json)
- **Frontend**: React
- **Deployment**: Docker, Docker Compose
- **Other**: Gunicorn for serving, Flake8 for linting

## Project Structure
- `server/`: Main Django server directory
  - `djangoapp/`: Django application with models, views, and REST APIs
  - `database/`: Node.js microservices for data management
  - `microservices/`: Additional services like sentiment analysis
  - `djangoproj/`: Django project settings
  - `djangoenv/`: Python virtual environment
- `frontend/`: React frontend application
- `deployment.yaml`: Kubernetes deployment configuration
- `Dockerfile`: Docker configuration for the server

## Setup Instructions
1. Ensure Docker and Docker Compose are installed
2. Navigate to the server directory
3. Run `docker-compose up` to start the services
4. For local development:
   - Activate the virtual environment: `source server/djangoenv/bin/activate`
   - Install dependencies: `pip install -r server/requirements.txt`
   - Run migrations: `python server/manage.py migrate`
   - Start the server: `python server/manage.py runserver`

## Usage
- Access the application through the frontend interface
- Use the REST APIs for backend interactions
- Microservices handle specific functionalities like sentiment analysis on reviews

## Contributing
This is a capstone project. For improvements, please follow standard development practices.
