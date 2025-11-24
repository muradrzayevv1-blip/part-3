# Django Polling Application

This project is a simple polling application built by following the official Django tutorial. It covers the basics of creating a Django project, developing an application, and writing automated tests.

This implementation specifically corresponds to the completion of **Part 3** of the tutorial, which introduces function-based views and URL mapping.

## Project Structure

- `mysite/`: The main Django project directory.
  - `settings.py`: Project settings.
  - `urls.py`: Main URL configuration.
- `polls/`: The polling application.
  - `models.py`: Data models for Questions and Choices.
  - `views.py`: Views to handle application logic.
  - `urls.py`: URL configuration for the polls app.
  - `tests.py`: Automated tests for the models and views. (Note: Tests are currently disabled/ignored as this version uses Part 3's simpler views.)
  - `templates/`: HTML templates for the user interface.
  - `static/`: Static files (CSS, images) for the app.
- `manage.py`: Django's command-line utility for administrative tasks.
- `db.sqlite3`: The SQLite database file.
- `.gitignore`: Specifies files to be ignored by Git.

## Getting Started

### Prerequisites

- Python 3.x
- pip

### Setup and Installation

1.  **Clone the repository (or download the source code):**

    ```bash
    git clone <repository-url>
    cd django-polls-tutorial
    ```

2.  **Create and activate a virtual environment:**

    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Install the dependencies:**

    ```bash
    pip install django
    ```

4.  **Apply the database migrations:**

    ```bash
    python manage.py migrate
    ```

### Running the Development Server

To start the local development server, run the following command:

```bash
python manage.py runserver
```

You can now access the application at `http://127.0.0.1:8000/polls/`.

### Running the Automated Tests

To run the suite of automated tests, use the `test` command:

```bash
python manage.py test polls
```

The tests will run and report on their success or failure. All tests included in this project should pass.
