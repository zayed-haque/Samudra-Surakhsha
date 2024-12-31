# SamudraSuraksha

SamudraSuraksha is a mobile application designed to provide recreational suitability and safety information for beach locations across India. Leveraging real-time data from INCOIS and Windy APIs, this application helps users make informed decisions about their beach visits by providing geospatial visualizations and safety notifications.

## Features

- **Multi-Platform Support**: Available on both Android and iOS.
- **Real-Time Data Integration**: Fetches and updates data on oceanic and meteorological conditions.
- **Machine Learning**: Provides safety assessments using ML models.
- **Geospatial Visualization**: Displays beach locations and data using Mapbox.
- **User Notifications**: Delivers personalized safety alerts and updates.
- **Personalized Profiles**: Users can save favorite beaches and track recently visited locations.
- **SOS Functionality**: Quick access to emergency contacts.
- **Search Functionality**: Search beaches based on name, location, or safety status.

---

## Architecture

Below is a high-level architecture diagram showcasing the interaction between various components in SamudraSuraksha:

![Architecture Diagram](literate-octo-fortnight/assests/architecture.png)

---

## User Journey Workflow

Below is a high-level workflow diagram showcasing the interaction among the user and the  various components in SamudraSuraksha:

![Workflow Diagram](literate-octo-fortnight/assests/Flow.png)

---



## Tech Stack

- **Frontend**: React Native
- **Backend**: Python with FastAPI
- **Database**: PostgreSQL with PostGIS
- **APIs**: INCOIS and Windy APIs
- **Geospatial Visualization**: Mapbox
- **Machine Learning**: Integrated safety models

---

## Prerequisites

- Docker
- Node.js and Yarn for frontend development
- Python 3.10 or higher for backend development

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/sandeepangh782/literate-octo-fortnight.git
cd sandeepangh782-literate-octo-fortnight
```

---

### Set Up Environment Variables

1. Copy the `.env.example` file to `.env` in the project root.
2. Fill in the required environment variables (e.g., `DATABASE_URL`, API keys, etc.).

---

### Start the Backend with Docker

1. Build and start the containers:
   ```bash
   docker-compose up --build
   ```

2. Access the backend API at `http://localhost:8000`.

3. To stop the containers:
   ```bash
   docker-compose down
   ```

---

### Run the Frontend

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   yarn install
   ```

3. Start the development server:
   ```bash
   yarn start
   ```

4. Follow the instructions to launch the app on your connected device or emulator.

---

## API Endpoints

- **GET /api/v1/beaches**: Fetches nearby beaches based on user location.
- **POST /api/v1/favorites**: Add a beach to favorites.
- **GET /api/v1/notifications**: Retrieves user notifications.

---

## Machine Learning Integration

The backend includes ML models (e.g., `safety_index_model.pkl`) for assessing beach safety based on various parameters such as wave height, weather, and UV conditions.

---

## Contributing

Contributions are welcome! Please fork this repository and create a pull request with your changes.

---

## Screenshots

### Home Screen
![Home Screen](literate-octo-fortnight/assests/homescreen.png)

### Beach Details Screen
![Beach Details Screen](literate-octo-fortnight/assests/BeachDetail.png)

### Search Screen
![Search Screen](literate-octo-fortnight/assests/Search.png)

### SOS Feature
![SOS Screen](literate-octo-fortnight/assests/EmergencyALert.png)

---