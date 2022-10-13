# Movie Rater

Full-stack movie rating demo with a Django REST API and a React frontend.

## About

This project lets authenticated users browse movies and submit a 1-to-5 star rating for each title. The backend exposes a Django REST Framework API, while the React app fetches the movie list and presents the UI for rating interactions.

## Key Features

- User registration with token auth
- Movie listing and rating endpoints
- One-rating-per-user-per-movie constraint
- React front end for browsing the catalog

## Architecture

- `django-movie-rater/` is the backend
- `react-movie-rater/` is the frontend
- Django models store movies and ratings

## Tech Stack

- Python
- Django
- Django REST Framework
- React
- JavaScript

## Prerequisites

- Python 3.x
- Node.js
- SQLite or another Django-compatible database

## Installation

```bash
cd django-movie-rater
pip install -r requirements.txt

cd ../react-movie-rater
npm install
```

## Configuration

- The React frontend currently hardcodes the backend URL and token in `src/App.js`
- The Django app uses the standard `manage.py` entry point

## How to Run

```bash
cd django-movie-rater
python manage.py runserver

cd ../react-movie-rater
npm start
```

## Example Usage

- Register a user against the Django API
- Fetch the movie list and submit a rating through the React frontend

## Project Structure

- `django-movie-rater/api/` - models, serializers, and viewsets
- `django-movie-rater/movierater/` - Django project settings
- `react-movie-rater/src/` - frontend UI

## Current Status

Functional prototype, but the React app contains a hard-coded API token and the workspace snapshot does not show a polished deployment story.

## Limitations

- Hard-coded authorization token in the React app
- No root env example
- No repo-level license

## License

No explicit license file was found at the repository root.
