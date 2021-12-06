# Udacity-Ci

We will use an existing application for convenience. If you'd like to use your own application, that's fine, but be aware there may be some differences. To use the suggested application, please fork and clone this repository.
Create the Circle CI config file.
Create three jobs with the following names: build, test, and analyze. Each job should have some common elements. For example, before doing anything that works with code, you will need to checkout. You may also have to install any dependencies needed to run the code or complete some task. Here are the commands we suggest running:

For the build job, npm run lint

For the test job, npm run test
For the analyze job, npm audit

Define a workflow that invokes each job in sequential order, where test depends on build and analyze depends on test.

Commit your new changes and watch the pipeline run.
You should see that the analyze job fails since some packages have security vulnerabilities.
