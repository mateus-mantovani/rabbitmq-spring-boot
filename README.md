# rabbitmq-spring-boot-examples

## How to run
The examples have profile context. Chose one example and get the profile name context to run with the flag --spring.profiles.active.

### Example - Tutorial 2
shell 1
java -jar target/rabbitmq-tutorials.jar --spring.profiles.active=work-queues,receiver

shell 2
java -jar target/rabbitmq-tutorials.jar --spring.profiles.active=work-queues,sender

### Example - Tutorial 3
shell 1
java -jar target/rabbitmq-tutorials.jar --spring.profiles.active=pub-sub,receiver \
    --tutorial.client.duration=60000
    
shell 2
java -jar target/rabbitmq-tutorials.jar --spring.profiles.active=pub-sub,sender \
    --tutorial.client.duration=60000
