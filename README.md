# simple-webapp-flask-revised

This is a simple web application using [Python Flask](http://flask.pocoo.org/)  

You can run the container using 
```docker pull csborle/my-simple-webapp-improved``` .
For more details regarding this image you can visit [Webapp flask](https://hub.docker.com/r/csborle/my-simple-webapp-improved)
  
  Below are the steps required to get this working on a base linux system.
  
  - Install all required dependencies
  - Install and Configure Web Server
  - Start Web Server
   
## 1. Update

    apt-get update

## 2. Install all required dependencies
  
  Python and its dependencies

    apt-get install -y python3

## 3. Install latest pip

    apt-get install python3-pip

   
## 4. Install and Configure Web Server

Install Python Flask dependency

    pip install flask

- Copy app.py or download it from source repository
- Configure database credentials and parameters 

## 5. Start Web Server

Start web server

    FLASK_APP=/opt/app.py flask run --host=0.0.0.0
    
## 6. Test

Open a browser and go to URL

    http://<IP>:5000                            => Welcome
    http://<IP>:5000/how%20are%20you            => I am good, how about you?



## Regarding building the image
Difference when building image using ubuntu vs python3.11 slim![image](https://github.com/nightfury000/simple-webapp-flask-revised/assets/83269908/8067aedd-920b-4c4a-8772-4511295d890a)

