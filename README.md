

# Simple Site: React + Django + SQLite

# Description
- Simple 'Note' App run with two containers:
    - Frontend app w/ Reacct
    - API and SQLite DB w/ Django

# How to Run with Docker Containers
- Make sure docker desktop is installed for non-Linux users!!! (Creates a linux vm so you can run containers).
- You need to build the images first with: ```docker-compose build``` (run where docker-compose.yaml is located).
    - Run the build commmand whenever you make changes to the code .

- Start the site with: 
    - ```docker-compose up``` (run where docker-compose.yaml is located)
    - Both containers (backend and frontend) will run
    - Go to localhost:3000
- ALWAYS remember to stop and remove containers with ```docker-compose down``` command.

# Add secret key for Django backend
- Create a ```.env``` file at /backend and add the key


# Folders:
## frontend
- React app
- Run without docker: ```npm start```

## backend
- Django api + SQLite database 
- Run without docker: ```python3 manage.py runserver```

## tutorial-env
- [Virtual Environments and Packages](https://docs.python.org/3/tutorial/venv.html)
- Python virtual env, activate with:
    - MacOS/Unix: ```source tutorial-env/bin/activate```
    - Windows: ```tutorial-env\Scripts\activate.bat```


# Resources
- [How to Dockerize a Django and React Application](https://www.honeybadger.io/blog/docker-django-react/)
- [Adding Custom Environment Variables](https://create-react-app.dev/docs/adding-custom-environment-variables/)
- [Writing your first Django app, part 1](https://docs.djangoproject.com/en/4.1/intro/tutorial01/)
- [Build a REST API in 30 minutes with Django REST Framework](https://medium.com/swlh/full-stack-with-django-and-react-react-afae36017852)
- [When to run a command in docker compose and when in dockerfile?](https://stackoverflow.com/questions/69036887/when-to-run-a-command-in-docker-compose-and-when-in-dockerfile)