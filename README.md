

# Simple Site: React + Django + SQLite


# How to Run
- Make sure docker desktop is installed for non-Linux users!!! (Creates a linux vm so you can run containers)

- Start the site with: 
    - ```docker-compose up``` (run where docker-compose.yaml is located)
    - Both containers (backend and frontend) will run
    - Go to localhost:3000
- ALWAYS remember to stop and remove containers with ```docker-compose down``` command.

- If changes are made to the django app or react app, make sure to run ```docker-compose build``` before running docker-compose up again. 

# Folders:
## sprite-animation (react app)
- Run: ```npm start```

## backend
- django api + sqlite database 
- Run: ```python3 manage.py runserver```

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