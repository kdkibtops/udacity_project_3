# Apllication Infrastructure

## AWS
### RDS Postgres
Application uses AWS RDS Postgres storing and retrieving user and feed info.

Database URI: `project3.cmlfaxhabm4x.us-east-1.rds.amazonaws.com`


### S3 Bucket
The frontend application assets are uploaded to a publicly accessible S3 bucket 

Bucket URL: `http://udagram-heidar.s3-website-us-east-1.amazonaws.com`

use this URL to access the website


### Elastic Beanstalk
it runs the server for hosting the application

EB URL: `http://heidar-dev.eba-2uwmteyp.us-east-1.elasticbeanstalk.com/`

## [Architecture](architecture.png)
1. Client access the frontend through S3 Bucket URL
2. Client submits a request
3. Request in handled by the api on Beanstalk and do fetches
4. API server manipulates/queries the RDS Database on AWS RDS
5. RDS returns needed data to server API
6. Server API sends response to frontend to client