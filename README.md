Level 1 : Create the Container to run the application
===========================================
* install dependencies (mysql/python3/uwsgi) in the container
* create a virtualenv and install the requirements for python (requirements.txt)
* runs migrate everytime the container starts
* use uwsgi to run the application in http mode
* modify the app to get the credentials for the DB externally

Level 2: Run the container using docker-compose
===========================================
* create docker-compose.yml
* create inject the necessary credentials to connect to the db
* map on port 80

Level 3 : Run the container using minikube on the EC2 instance
===========================================
* Configure minikube on the EC2 instance
* Create the deployment.yml necessary to run the container in minikube, connecting to the external RDS
* optional : configure and create the ingress to access the application from the port 80 of the EC2 instance
