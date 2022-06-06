# Infrastructure:
### This web application consists of two parts:
1- Frontend called udagram-frontend was built and uploaded on the S3 bucket on the Amazon Web Services
2- Backend called udagram-api was built and uploaded on the Elastic beanstalk
3- RDS Relational Database was created and connected to the backend waiting for users to signup and login
4- Circleci connected to the github repo and waiting for any changes to test, build and deploy the project one more time

### Process:
The client browses to the URL of the web application. First he uses the frontend and tries to uses (like he tries to login to his page) the frontend (S3 Bucket) sends a request to the backend (Elastic beanstalk), the backend (Elastic beanstalk) sends a request to the (RDS) database. 
the (RDS) database respondes and retrieves the necessary data, sends it to the backend (Elastic beanstalk), the backend (Elastic beanstalk) sends the proccessed data to the frontend (S3 Bucket) finally the frontend (S3 Bucket) displays the data on the client's browser.


## URLs:
1- S3 bucket FrontEnd: http://udagram-frontend-clientside.s3-website-us-east-1.amazonaws.com

2- Elastic beanstalk API: udagram-api-env1.eba-bgwkwkt7.us-east-1.elasticbeanstalk.com

