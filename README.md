# Jenkins configuration for Spandx Deployment Service

To create a new Jenkins Job from the template, run:

```
java -jar jenkins-cli.jar -s JENKINS_PATH create-job JOBNAME < config.xml
```

## Configuration

### Jenkins

Standard Jenkins CLI flags can be used for authentication purposes. Checkout https://jenkins.io/doc/book/managing/cli/ for details about configuring Jenkins CLI. 

To install Jenkins CLI and get a list of CLI options visit the `/cli` page of your local jenkins installation

### Job Config

To configure individual job properties, visit `/job/JOBNAME/configure` page from Jenkins once you have imported the job.

## Example

Considering that Jenkins is running at http://localhost:8080 and you have a .jenkins-cli file configured for your local jenkins installation, you can create a new Jenkins job using Jenkins CLI by running:

```
java -jar jenkins-cli.jar -auth @.jenkins-cli -s http://localhost:8080/ create-job SDS < config.xml
```
