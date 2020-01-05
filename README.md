# RabbitMqProject

- Install RabbitMq from Homebrew manager https://www.rabbitmq.com/install-homebrew.html
  
  The server can then be started with rabbitmq-server.

1. HelloWorld with RabbitMq (**helloWorld branch**)
  
   "This project is a producer that sends a single message, and a consumer that receives messages and prints them out."
   https://www.rabbitmq.com/tutorials/tutorial-one-java.html

    - Steps
      - Create a maven project
      - Add some dependencies on your pom (loggers and rabbitmq dependency)
      - Create producer class
      - Create consumer class
      - Download the jar files (slf4j simple and api, rabbitmq also)
      - Run the rabbitmq server (inside sbin folder on your local)
        - $ ./rabbitmq-server (Server)
      - Compile (javac) and run them (java) with the following commands (put the jars inside of src/main/java/.)
        - $ java -cp .:amqp-client-5.8.0.jar:slf4j-api-2.0.0-alpha1.jar:slf4j-simple-2.0.0-alpha1.jar Recv (Consumer)
        - $ java -cp .:amqp-client-5.8.0.jar:slf4j-api-2.0.0-alpha1.jar:slf4j-simple-2.0.0-alpha1.jar Send (Producer)
