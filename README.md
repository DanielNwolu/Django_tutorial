# Django Polls App (Tutorial Part 3)

This project is a Django web application following the official [Django tutorial](https://docs.djangoproject.com/en/stable/intro/tutorial03/), up to the end of Part 3. It implements a simple polling app where users can view questions and vote.

## Features Implemented
- **Django project and app setup**: Project created, `polls` app added.
- **Models**: `Question` and `Choice` models defined (see `polls/models.py`).
- **Database migrations**: Initial migrations created and applied.
- **Admin site**: Admin enabled, models registered for easy data entry.
- **Views**: Four main views:
  - Index (list of latest questions)
  - Detail (question and choices)
  - Results (voting results)
  - Vote (handles voting)
- **Templates**: HTML templates for index and detail pages, using Django’s template language.
- **URL routing**: Clean, named URLs for each view, using namespacing for the `polls` app.
- **Error handling**: 404 error if a question does not exist.

## Getting Started

### Prerequisites
- Python 3.8+
- [Poetry](https://python-poetry.org/) (for dependency management)
- (Optional) Virtual environment (recommended)

### Setup Instructions
1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd <repo-folder>
   ```
2. **Install dependencies**
   ```bash
   poetry install
   ```
3. **Apply migrations**
   ```bash
   poetry run python manage.py migrate
   ```
4. **Create a superuser (for admin access)**
   ```bash
   poetry run python manage.py createsuperuser
   ```
5. **Run the development server**
   ```bash
   poetry run python manage.py runserver
   ```
6. **Access the app**
   - Visit [http://127.0.0.1:8000/polls/](http://127.0.0.1:8000/polls/) to see the polls app.
   - Visit [http://127.0.0.1:8000/admin/](http://127.0.0.1:8000/admin/) to manage questions and choices.

## Project Structure
- `polls/` – Django app with models, views, templates, and URLs
- `polls/templates/polls/` – App-specific HTML templates
- `manage.py` – Django’s command-line utility
- `README.md` – This file

## References
- [Django Tutorial Part 3](https://docs.djangoproject.com/en/stable/intro/tutorial03/)
- [Django Documentation](https://docs.djangoproject.com/en/stable/)

---
*This project is a learning exercise and a starting point for further Django development.* 