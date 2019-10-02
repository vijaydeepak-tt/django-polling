# POLLING
    A framework polling web application developed with Django.

### Set UP:
1. Install python from https://www.python.org/, along with python it will installs pip - a python package manager.
2. Run "pip install pipenv" to create a virtual environment.
3. After installing pipenv, run "pipenv shell" from the current project directory to create a virtual environment for the project. It will creates a folder in the name of the project inside the folder ".virtualenvs" in the Users folder in C: drive.
4. Then run "pipenv install django" in the current directory to install django package inside the virtual environment project folder.
5. Next run "django-admin startproject polling" to create project inside our directory.
6. After that, go to polling directory ( cd polling ) and then run "python manage.py runserver" to run the server.
7. We have to add some of the required things such as admin, auth, session and contenttypes, run "python manage.py migrate" to create the required tables in the SQlite DB.
8. Next, run "python manage.py startapp polls" to create a polls app. It will creates an app directory with some of the required files.
9. Create models, add "polls.apps.PollsConfig" line of code in polling/settings.py under installed apps ,then run "python manage.py makemigrations polls" to create migration file.
10. Run "python manage.py migrate" to create the tables in database.
11. "python manage.py shell", this cmd is useful to run model actions in the terminal.
12. Run "python manage.py createsuperuser" to create a super user for the project.
13. Run "python manage.py startapp pages" cmd to create the starting pages.

Note: If your system not provides permission to activate the virtual environment run "powershell Set-ExecutionPolicy RemoteSigned". Form more info https://stackoverflow.com/questions/4037939/powershell-says-execution-of-scripts-is-disabled-on-this-system
