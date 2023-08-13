# Microservices

## Virtual Environment
### To create a virtual environment
python3 -m pip install virtualenv
python3 -m virtualenv .
source bin/activate

# to deactivate
deactivate

## to install pip
python3 -m pip install --upgrade pip
python3 -m pip install --user --upgrade pip

## To install dependencies
pip install -r requirements.txt

## To run the application
python app.py

## Docker
### To build the image
docker build -t microservices .

### To run the image
docker run -d -p 5000:5000 microservices

### To stop the image
docker stop microservices

### To remove the image
docker rm microservices

### To push the image to docker hub
docker tag microservices <dockerhub_username>/microservices
docker push <dockerhub_username>/microservices

### To pull the image from docker hub
docker pull <dockerhub_username>/microservices

## to open the flask app in browser
http://localhost:5000/

## To run the tests
python -m pytest