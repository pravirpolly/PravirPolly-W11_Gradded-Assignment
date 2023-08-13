# Microservices

# To build the image
docker build -t microservices .

# To run the image
docker run -d -p 5000:5000 microservices

# To push the image to docker hub
docker tag microservices <dockerhub_username>/microservices
docker push <dockerhub_username>/microservices

# To pull the image from docker hub
docker pull <dockerhub_username>/microservices