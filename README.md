# Project-8b-Using-Docker-to-containerize-Flask-Applications

- We use docker to containerize the flask application from project 8a.    

# Steps:
1. create a docker-compose.yaml file
2. create a requirements.txt file which contains the version of the packages used in your app.py
3. create a Dockerfile which acts to instruct docker on what steps to take for files in that directory 
 - in our file we set the working directory and copy the current directory into the contain using 'COPY'
 - we then run the requirements.txt file which contains the version of the packages used in your app.py
 - we expose port 5000 since this will be the port on the local computer being used 
 - state an entry point and command which allows the application to run  
