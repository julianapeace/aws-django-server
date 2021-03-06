![alt text](https://herc.one/wp-content/uploads/2018/03/hercLogoFront.png "Herc Logo") 
# Django Test Server
### For Mock Endpoints
-------
## Database:
- Postgresql (Version 10)

MacOS Tools for the Database:
- Postgres.app[link](https://postgresapp.com/
- Postico[link](https://eggerapps.at/postico/)

------

### Documentation

#### In order to run this repo, you will need:
- python 3.6
- pip
- pipenv
- a postgres database running on your local envionment

1.  Check if you have python by running `python3 --v`.
2.  Install pip [here](https://pip.pypa.io/en/stable/installing/)
3. Install pipenv with `pip install pipenv`
4.  Open Postgres and click `initialize`
5. Open Postico. Create a database called "hercules."
6. git clone this repository
7. cd into the repository. Run "Pipenv install". This spawns a virtual environment. It will also look at the Pipfile(located in the root directory) and install all the dependencies listed there.
8. run `pipenv run ./manage.py migrate`
9. run `pipenv run ./manage.py createsuperuser`
10. create your superuser login credentials. 
11. Run the server with `pipenv run ./manage.py runserver`

##### Did you make a change to your database models?
- Update your migration files with `pipenv run ./manage.py makemigrations`
- Then run `pipenv run ./manage.py migrate`  
 

