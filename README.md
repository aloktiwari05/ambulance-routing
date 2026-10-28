# Ambulance Routing System

A Django web application for planning ambulance routes efficiently and identifying nearby hospitals in emergency scenarios.

## Features

- Route optimization between start and destination locations
- Google Maps integration for live route and distance data
- Nearby hospital detection by radius
- Emergency and standard route modes
- Simple web-based interface

## Tech Stack

- Python 3.11+
- Django 5.x
- Google Maps API
- geopy
- Bootstrap-style frontend assets

## Project Structure

- `ambulance_routing/` — Django project files
- `routing/` — app logic and route-related views
- `static/` — CSS and static assets
- `manage.py` — Django management entry point

## Prerequisites

- Python 3.11 or later
- pip
- A Google Maps API key

## Local Setup

1. Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   ```

2. Install project dependencies:
   ```bash
   pip install -r ambulance_routing/requirement.txt
   ```

3. Create a local `.env` file from the example:
   ```bash
   copy .env.example .env
   ```
   On Linux/macOS:
   ```bash
   cp .env.example .env
   ```

4. Update the values in `.env` with your own credentials.

5. Run the development server:
   ```bash
   python ambulance_routing/manage.py runserver
   ```

## Environment Variables

The application expects the following variables in a local `.env` file:

```env
DJANGO_SECRET_KEY=your-strong-random-secret
DJANGO_DEBUG=True
DJANGO_ALLOWED_HOSTS=localhost,127.0.0.1
GOOGLE_MAPS_API_KEY=your_google_maps_api_key
```

## Security Notes

- Never commit the real `.env` file to GitHub.
- Keep API keys and secrets private.
- Use `.env.example` as the safe template that can be shared publicly.

## License

This project is intended for academic or internal use unless otherwise specified by the owner.
