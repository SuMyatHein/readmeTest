#Git Clone
git clone https://github.com/WPPM/Django.git
cd django

#Create Virtual Environment
py -m venv .venv

#Activate Virtual Environment
.venv\scripts\activate

#Install Modules
pip install -r requirements.txt

#Run
python manage.py runserver

#Database Table Migrate
python manage.py migrate
python manage.py makemigrations

#Run script to load outputsimilar.csv data
python manage.py runscript load_outputsimilar

#Create Superuser
python manage.py createsuperuser

#Run
python manage.py runserver


To run django project:

1) git clone https://github.com/SuMyatHein/csvdjango.git
2) python -m venv .venv
3) .venv\scripts\activate
4) pip install -r requirements.txt
5) python manage.py runserver

To create mysql database using xampp:

1) Click New => create new database : edogawa_testdb
2) Import SQL files.
3) Change database name in edogawachildabuse>>settings.py: 
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'edogawa_testdb',
        'USER':'root',
        'PASSWORD':'',
        'HOST':'localhost',
        'PORT': '3306',
    }
}
