# Cold Email Generator

## Overview
A Flask web application that generates cold emails and follow-ups using AI. Users can input a company website URL, prospect details, and email goals to generate personalized cold outreach emails. Supports Google Gemini API for AI generation with a basic fallback.

## Recent Changes
- 2026-02-09: Initial import and setup - installed packages, created templates, configured workflow

## Project Architecture
- **Backend**: Flask (Python 3.11) with SQLAlchemy (SQLite)
- **Frontend**: Jinja2 templates with Bootstrap 5, Font Awesome icons
- **AI**: Google Gemini API (optional, configured via Settings page)
- **Web scraping**: BeautifulSoup4 + requests for company website data

### Key Files
- `app.py` - Main Flask application with routes, models, and business logic
- `main.py` - Entry point for gunicorn
- `templates/base.html` - Base template with navbar
- `templates/dashboard.html` - Main form and results display
- `templates/settings.html` - Gemini API key configuration
- `static/css/style.css` - Custom styles

### Features
- Website scraping for company info
- Cold email + 2 follow-up generation
- Rate limiting (5 requests/hour per IP)
- Gemini API integration (optional)
- Tone selection (Professional, Casual, Friendly, Urgent)

## User Preferences
- No specific preferences recorded yet
