# Build the Docker image for a Python Flask app
docker build -t hello-python .

# Run the Docker image
docker run -it --rm hello-python

# Check if the web page was deployed properly
curl 127.0.0.1:5000