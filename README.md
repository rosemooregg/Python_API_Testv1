# Python_API_Testv1
In this example, the Python script validate_apis.py defines a list of API URLs to validate. It uses the requests library to send HTTP GET requests to these URLs and checks the response for HTTP errors. The Dockerfile specifies a Python 3.8 base image, sets up a working directory, copies the Python script into the container, installs any required dependencies from a requirements.txt file, exposes port 80 (in case you need to run a web service), and finally runs the Python script when the container is launched.

You can customize the list of API URLs in the Python script and adjust the Dockerfile according to your specific requirements. To build and run the Docker container, follow these steps:

Place the Python script and Dockerfile in the same directory.
Create a requirements.txt file if you have any Python dependencies and list them there.
Build the Docker image using the docker build command.
Run the Docker container with the docker run command.
This setup allows you to validate multiple API URLs within a Docker container, making it easy to manage and deploy your API validation script.
