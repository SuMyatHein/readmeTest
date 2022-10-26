# To run django project:
#### Git Clone
    git clone https://github.com/WPPM/Django.git
####
    cd django
#### Create Virtual Environment
    py -m venv .venv

#### Activate Virtual Environment
    .venv\scripts\activate

#### Install Modules
    pip install -r requirements.txt

#### Run
    python manage.py runserver

#### Database Table Migrate
    python manage.py migrate
####
    python manage.py makemigrations

#### Run script to load outputsimilar.csv data
    python manage.py runscript load_outputsimilar

#### Create Superuser
    python manage.py createsuperuser

#### Run
    python manage.py runserver
