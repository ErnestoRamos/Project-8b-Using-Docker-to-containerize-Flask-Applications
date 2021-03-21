# Project-8b-Using-Docker-to-createcontainer-Flask-Applications

- We use docker to containerize the flask application from project 8a.    

# Steps:
1. create a docker-compose.yaml file
2. create a requirements.txt file which contains the version of the packages used in your app.py
3. create a Dockerfile image which acts to instruct docker on what steps to take for files in that directory 
  - in our file we set the working directory and copy the current directory into the contain using 'COPY'
  - we then add a line to run the requirements.txt file which contains the version of the packages used in your app.py
  - we expose port 5000 since this will be the port on the local computer being used 
  - state an entry point and command which allows the application to run  
4. in your linux terminal, we have to build the container using: 'docker build -t testapp:latest .'
  - note that testapp can be any name
5. we then use docker-compose up to start the container and then go to localhost:5000 to view your API
6. finally, save your docker container in your selected directory using 'docker save testapp > testapp.tar' 

![image](https://user-images.githubusercontent.com/56518821/111897346-d0eb3380-89f5-11eb-800a-16806561c3f3.png)
