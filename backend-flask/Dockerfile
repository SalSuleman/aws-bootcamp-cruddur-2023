FROM python:3.10-slim-buster

# Inside Container
# create new folder inside container
WORKDIR /backend-flask

# Outside Continer -> Inside container
# this contains the libraries we want to install to run the app
COPY requirements.txt requirements.txt

# Inside Container
# this installs the python libraries used for the app
## RUN creates a layer in the container
RUN pip3 install -r requirements.txt

# Outside container -> Inside Container
COPY . .

# Set env vars inside the container
ENV FLASK_ENV=development

EXPOSE ${PORT}

# command to run flask on port 4567
## CMD runs a command inside the container when it starts up
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]