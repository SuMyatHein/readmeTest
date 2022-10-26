# To run django project:
#### Git Clone
    git clone https://github.com/WPPM/Django.git
(or)
####
    git clone https://github.com/SuMyatHein/csvdjango.git
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

#### To create mysql database using xampp:
Click New => create new database : edogawa_testdb

#### Method 1 (Data will be the same previous database as user, uploaded data and outputsimilar data)
1.Import SQL files.

2.Change database name in edogawachildabuse>>settings.py: 
```
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
```

#### Method 2 (New Database)
1.Database Table Migrate
####
	python manage.py migrate

####
	python manage.py makemigrations
		
2.Run script to load outputsimilar.csv data
####
	python manage.py runscript load_outputsimilar

3.Create Superuser
####
	python manage.py createsuperuser

#### Run
    python manage.py runserver



