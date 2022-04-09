# Infrastructure Description

Udagram uses 3 AWS services:

- Elastic Beanstalk
- RDS
- S3

### Elastic Beanstalk

AWS Elastic Beanstalk is an easy to use service for hosting web applications, EB is used to run Udagram API on an EB environment with required environment variables as database connection strings, JWT secret key, etc. EB provides a way to hide sensitive variables from the code itself.

### RDS

Now, the back-end API requires a database that must be available online whenever the back-end is requested to save data, RDS is a service that is provided by AWS to create databases online, whenever the user makes a request that needs to save or pull data from the database, RDS is available to do so.

### S3

S3 is a service that is all about saving files on AWS servers, but it's also used to serve static websites that doesn't require server-side rendering. S3 is used to host a production built front-end applications, and it communicates with the backend via JavaScript HTTP requests.

![](https://i.imgur.com/Rov1k3K.png)
