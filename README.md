# SaaS Billing System

This project is a SaaS (Software as a Service) billing system built with Django. It provides functionalities to manage clients, products, campaigns, payments, invoices, and reports through a web-based dashboard interface.

## Features

- Client management: Create, update, and view client details.
- Product management: Manage products and packages.
- Campaign management: Create and track marketing campaigns.
- Payment processing: Handle payments and generate invoices.
- Reporting: Generate daily, monthly, and yearly reports.
- User authentication and authorization.
- Responsive UI using Bootstrap 5.

## Technology Stack

- Backend: Django (Python)
- Frontend: Django Templates with Bootstrap 5
- Database: SQLite (default, can be changed)
- Styling: Bootstrap 5 via django-bootstrap5 package

## Installation

1. Clone the repository:

   ```
   git clone https://github.com/coolguy-sree/saas-billing.git
   cd saas-billing-system-saas
   ```

2. Create and activate a virtual environment:

   ```
   python -m venv venv
   venv\Scripts\activate   # On Windows
   source venv/bin/activate  # On Linux/macOS
   ```

3. Install dependencies:

   ```
   pip install -r requirements.txt
   ```

4. Apply migrations:

   ```
   python manage.py migrate
   ```

5. Run the development server:

   ```
   pipenv run python manage.py runserver
   ```

6. Access the application at `http://127.0.0.1:8000/`

## Notes

- The project uses the `django-bootstrap5` package for Bootstrap integration. Ensure templates load the tag library as `{% load django_bootstrap5 %}`.
- If you encounter template tag errors related to `bootstrap5`, verify the tag library name and restart the development server to clear caches.

## Testing

- Manual testing can be done by navigating through the dashboard pages and verifying UI components and functionalities.
- Automated tests can be run using:

  ```
  python manage.py test
  ```

## License

This project is licensed under the MIT License.
