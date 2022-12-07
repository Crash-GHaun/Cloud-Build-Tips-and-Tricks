# Using Cloud Build to Deploy a scheduler and use source control for schedule. 

## Requirements

CloudBuild Service Account will need access to list, create, and update jobs!

## Description

This is an example of how to use Cloud Build to deploy a Job on Cloud Scheduler that points to a function. The use case here is you have a function that is being deployed in multiple environments and you want to use source control to modify the schedule, etc. 

The steps this cloudbuild + bash file takes are:

1. Set's environment variables
2. Grabs the Service Account and URI of a cloud function and sets it to a variable.
3. Checks if a job exists already, if not it creates the job.
4. If the job exists it updates the existing job. 

Anyways, short and straight to the point. Not sure what else to write here. 
