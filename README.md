This is a very simple Java and Spring application demonstrating the use of RabbitMQ on Cloud Foundry.

## Deploying to Cloud Foundry ##

After installing in the 'cf' [command-line interface](http://docs.cloudfoundry.com/docs/using/managing-apps/cf/) for Cloud Foundry, targeting a Cloud Foundry instance, and logging in, the application can be pushed using these commands:

- git clone this repo
- cd spring-amqp-example
- mvn package
- cf marketplace
    find the messaging service
- cf create-service cloudamqp lemur rabbitmq
- cf push rabbitmq-spring
