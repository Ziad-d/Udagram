# Pipeline Process

Udagram uses CircleCI as a pipeline, CircleCI's giant servers are helpful for deploying new versions fast, just for an example, the production build of the front-end app contains more than 300 files! this amount of files is difficult for normal internet connections to handle every time we want to make a small change to the app.

#### Installing Orbs

CircleCI offers Orbs, a way to import and install common used tech stack with no manual configuring required, Udagram uses the following orbs:-

- node@5.0.1
- aws-cli@1.3.1
- aws-elastic-beanstalk@2.0.1

#### Initializing The Frontend Web Application

CircleCI installs the node dependencies and creates a production build of the Angular web application, then uses the AWS CLI to deploy the build to S3.

#### Initializing The Backend API

CircleCI installs the node dependencies and creates a production build of the express application, then uses the EB CLI to deploy the build to EB.

![](https://i.imgur.com/hOJZGqp.png)
