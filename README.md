# Django Polls Application

![CI](https://github.com/cb0tt/swe1-app/actions/workflows/django.yml/badge.svg)
[![Coverage Status](https://coveralls.io/repos/github/cb0tt/swe1-app/badge.svg?branch=main)](https://coveralls.io/github/cb0tt/swe1-app?branch=main)

A Django web application for managing polls, deployed on AWS Elastic Beanstalk.

## Features

- Poll creation and voting system
- Admin interface for managing polls
- AWS Elastic Beanstalk deployment
- Continuous Integration with GitHub Actions
- Code coverage tracking with Coveralls

## Development

### Requirements

- Python 3.11
- Django 5.2.6
- Gunicorn

### Installation

```bash
# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Run development server
python manage.py runserver
```

### Testing

```bash
# Run tests
python manage.py test

# Run tests with coverage
coverage run manage.py test
coverage report
```

### Code Quality

```bash
# Format code with Black
black .

# Lint with Flake8
flake8 .
```

## Deployment

This application is configured for deployment on AWS Elastic Beanstalk.

### Create Deployment Package

```bash
git archive -o ../django_app_deploy.zip HEAD
```

Upload the ZIP file through the Elastic Beanstalk console.


