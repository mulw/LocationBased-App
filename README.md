Location-Based Web Application with Django and GeoDjango
Overview

This project is a Django-based web application focusing on location-based services, powered by GeoDjango. It enables users to find nearby shops by leveraging GeoDjango's geospatial functionalities.
Prerequisites

Before you begin, ensure you have met the following requirements:

    Python (3.5 and above)
    Django Web Framework (2.1 and above)
    GeoDjango Dependencies:
        GEOS
        GDAL
        PROJ.4
    PostgreSQL and PostGIS Database along with Docker

For detailed installation instructions, please refer to the GeoDjango documentation.
Installation

To install Location-Based Web Application, follow these steps:

    Clone the repository:


git clone https://github.com/mulw/LocationBased-App.git
cd LocationBased-App

Create a virtual environment:


python3 -m venv env
source env/bin/activate

Install Django and other dependencies:


pip install -r requirements.txt

Set up the PostgreSQL database:

    Update the DATABASES settings in settings.py with your PostgreSQL credentials.
    Run migrations: python manage.py makemigrations and python manage.py migrate.

Create a superuser:


    python manage.py createsuperuser

    Add initial data:
    Use a data migration to add initial demo data to your application. Obtain real-world data from Overpass Turbo and save it as data.json in your project’s root folder. Then create an empty migration and run it.

Usage

To run the Location-Based Web Application, follow these steps:

    Run the development server:


    python manage.py runserver

    Access the application:
    Navigate to http://localhost:8000/ in your web browser to access the application.

    Login as admin:
    Use the superuser credentials created earlier to access the admin interface.

    Explore nearby shops:
    Use the application interface to explore nearby shops displayed using GeoDjango's geospatial functionalities.

Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

    Fork the project.
    Create your feature branch (git checkout -b feature/AmazingFeature).
    Commit your changes (git commit -m 'Add some AmazingFeature').
    Push to the branch (git push origin feature/AmazingFeature).
    Open a pull request.
