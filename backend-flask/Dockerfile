FROM python:3.10-slim-buster

# inside container
# make a new folder inside container
WORKDIR /backend-flask

# outside container -> inside container
# this contains the libraries we want to install to run the app
COPY requirements.txt requirements.txt

# inside container 
# install the python images used for the app
RUN pip3 install -r requirements.txt

# outside container -> inside container 
# . means everything in the current directory
# first period . -backend-flask (outside container)
# second period ./backend-flask (inside container)
COPY . .

# set enviornment variables (env vars)
# these are set inside the container and will remain set when container is running
ENV FLASK_ENV=development

EXPOSE ${PORT}

# command (cmd)
# python3 -m flask run --host=0.0.0.0 --port=4567 
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]