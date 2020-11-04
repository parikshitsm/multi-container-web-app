# multi-container-web-app
This application shows how a web-application can be deployed on multiple docker containers. This is an initial working version.
In this application we have 6 different running docker containers where every container hosts an individual service. 
Below are the service details : 
  - Nginx
  - Client
  - API (server)
  - Postgres
  - Redis
  - Worker
  
# Steps to run the application
Under root directory look out for docker-compose.yml file. From command prompt execute below command from root project directory.

    docker-compose up
  
This shall start all docker containers respective to individual service. Once done verify if all containers are up & running by below command : 

    docker ps
  
Now open browser and check if below url is working as expected : 

  http://localhost:3050/
  
 This shall open the React application. This is a simple Fibonacci series application where user can enter any specific index as per need & verify if the application calculates    correct fibonacci value for the index. Example : Fibonacci series is as below : 
 
 1 1 2 3 5 8 13 21 34 .....
 
So if user enters index as 5 => corresponding value of 8 should be returned by the application and displayed the same on screen. 
Below is the sample output visible on screen.
 
Enter your index:                     Submit

Indexes I have seen:
5, 7, 8

Calculated Values:
For index 5 I calculated 8
For index 7 I calculated 21
For index 8 I calculated 34
 

  
