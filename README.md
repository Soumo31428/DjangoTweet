<<<<<<< HEAD
# Simplified Tweet Application

A clean and simplified Django application for creating and managing tweets.

## Summary

This is a lightweight Twitter-like application built with Django that allows users to register, create tweets with optional photos, and interact with content. The application features a clean, responsive design and follows Django best practices with a well-organized project structure.

## Tech Stack

- **Backend**: Django 3.0.5 (Python 3.6+)
- **Database**: SQLite3
- **Image Processing**: Pillow 9.5.0
- **Frontend**: HTML, CSS, Bootstrap
- **Authentication**: Django's built-in authentication system

## Features

- User registration and authentication
- Create, read, update, and delete tweets
- Upload photos with tweets
- Admin interface for managing content
- Responsive design

## Requirements

- Python 3.6+
- Django 3.0.5
- Pillow 9.5.0

## Installation

1. Clone or download the repository
2. Navigate to the project directory:
   ```
   cd simplified_tweet_project/tweet_project
   ```
3. Install the required packages:
   ```
   pip install -r requirements.txt
   ```
4. Apply database migrations:
   ```
   python manage.py migrate
   ```
5. Create a superuser (optional):
   ```
   python manage.py createsuperuser
   ```
6. Start the development server:
   ```
   python manage.py runserver
   ```

## Usage

After starting the development server, visit `http://127.0.0.1:8000/` in your browser.

### Key URLs

- Home page (redirects to tweet list): `http://127.0.0.1:8000/`
- Tweet list: `http://127.0.0.1:8000/tweet/`
- Create a new tweet: `http://127.0.0.1:8000/tweet/create/`
- Register a new user: `http://127.0.0.1:8000/tweet/register/`
- Login: `http://127.0.0.1:8000/accounts/login/`
- Admin interface: `http://127.0.0.1:8000/admin/`

### Default Admin Account

Username: admin
Password: admin

## Project Structure

```
tweet_project/
├── tweet_project/          # Django project settings
├── tweet/                  # Main tweet application
├── templates/              # Base templates and registration templates
├── static/                 # Static files (CSS, JS, images)
├── media/                  # Uploaded media files
├── db.sqlite3             # SQLite database
├── manage.py              # Django management script
├── requirements.txt       # Project dependencies
└── README.md              # This file
```

## License

This project is open source and available under the MIT License.
=======
# DjangoTweet
>>>>>>> d0643c29956f05d9313a5abf487ad37a36a0dc64
