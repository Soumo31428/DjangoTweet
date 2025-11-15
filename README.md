
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

- Python 3.6 or higher
- Django 3.0.5
- Pillow 9.5.0 (for image processing)
- Git (for version control)

## Setup and Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Soumo31428/DjangoTweet.git
cd DjangoTweet
```

### 2. Set Up Virtual Environment (Recommended)

Create and activate a virtual environment to isolate project dependencies:

**On Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

**On macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

Install all required packages from the requirements.txt file:

```bash
pip install -r requirements.txt
```

### 4. Database Setup

Apply database migrations to set up the database schema:

```bash
python manage.py migrate
```

### 5. Create a Superuser (Optional)

Create an admin account to access the Django admin interface:

```bash
python manage.py createsuperuser
```

Follow the prompts to set a username, email, and password.

### 6. Collect Static Files

Collect all static files to the STATIC_ROOT directory:

```bash
python manage.py collectstatic --noinput
```

### 7. Run the Development Server

Start the Django development server:

```bash
python manage.py runserver
```

The application will be available at `http://127.0.0.1:8000/`

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

## Project Configuration

### Static Files

The project uses Django's static files framework to serve CSS, JavaScript, and image assets:

- `STATIC_URL`: `/static/`
- `STATICFILES_DIRS`: Points to the local [static/](file:///c:/Users/svk97/OneDrive/Desktop/Django%20Tweet/simplified_tweet_project/tweet_project/static/) directory
- `STATIC_ROOT`: [staticfiles/](file:///c:/Users/svk97/OneDrive/Desktop/Django%20Tweet/simplified_tweet_project/tweet_project/staticfiles/) directory for collected static files

### Media Files

User-uploaded content (such as tweet images) is stored in the [media/](file:///c:/Users/svk97/OneDrive/Desktop/Django%20Tweet/simplified_tweet_project/tweet_project/media/) directory:

- `MEDIA_URL`: `/media/`
- `MEDIA_ROOT`: Points to the local [media/](file:///c:/Users/svk97/OneDrive/Desktop/Django%20Tweet/simplified_tweet_project/tweet_project/media/) directory

### Database

The project uses SQLite as the default database, stored in [db.sqlite3](file:///c:/Users/svk97/OneDrive/Desktop/Django%20Tweet/simplified_tweet_project/tweet_project/db.sqlite3). For production deployments, you may want to configure a different database backend in [settings.py](file:///c:/Users/svk97/OneDrive/Desktop/Django%20Tweet/simplified_tweet_project/tweet_project/tweet_project/settings.py).

## Troubleshooting

### Common Issues

1. **ModuleNotFoundError**: Make sure you've activated your virtual environment and installed dependencies with `pip install -r requirements.txt`

2. **Database migration errors**: Run `python manage.py migrate` to apply any pending migrations

3. **Static files not loading**: Run `python manage.py collectstatic` to collect static files

4. **Permission denied errors**: On Unix-based systems, you may need to adjust file permissions

### Development Best Practices

1. Always use a virtual environment
2. Keep dependencies updated in requirements.txt
3. Run tests before committing changes
4. Follow Django's coding conventions

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

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the MIT License.

