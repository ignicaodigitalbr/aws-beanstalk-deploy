# aws-beanstalk-deploy
Automated deploy for AWS ElasticBeanstalk through bitbucket pipelines.

## Requirements
To use that script you will need to use a bitbucket pipeline.
We use release branchs to deploy our applications following a default style: `release-v0.0.0.0-prod` and producing `v0.0.0.0-prod` as deployed version.
Some environment variables are required to upload our application:
* `EB_APPLICATION_NAME` that is your application name
* `EB_APPLICATION_ENVIRONMENT` that is your ElasticBeanstalk environment
* `EB_BUCKET_S3` that is a temporary bucket responsible to deliver a .zip to ElasticBeanstalk

## Running

Run that awesome script is more simple than walk in a cloud: `python deploy.py` and all the magician happen :p
