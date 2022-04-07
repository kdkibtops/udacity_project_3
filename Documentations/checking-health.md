# Elastic beanstalk (EB) application:
Steps to check the health of the EB application

1. Connect EB CLI to the enviroment using `eb use udagramheidar-env`
2. Check health using `eb health`
3. A table will be available with  information about the servers runnning the application.
3. Health should be `OK` otherwise, you have to check the logs to know the cause of the problem with the application.