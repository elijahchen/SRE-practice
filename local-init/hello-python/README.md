# Build the Docker image for a Python Flask app
docker build -t hello-python .

# Run the Docker image
docker run -p 5000:5000 hello-python

# Check if the web page was deployed properly
curl 127.0.0.1:5000

# Login to docker hub
docker login

# Docker push <username>/hello-python
docker push 0xelijah/hello-python:v1

# Docker pull <username>/hello-python:tag
docker pull 0xelijah/hello-python:v1

# Prepare the image locally with relevant tags
docker tag hello-python:latest 0xelijah/hello-python:v1

# Push the prepped image to the repository namespace
docker push 0xelijah/hello-python:v1

# Pull the image just to check
docker pull 0xelijah/hello-python:v1
