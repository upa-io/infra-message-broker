#Run container for rabbitMq 

docker run -d --hostname message-broker-dev --name message-service-bus-broker-dev -p 15672:15672 -p 5672:5672 -p 5671:5671 -e RABBITMQ_DEFAULT_USER=guest -e RABBITMQ_DEFAULT_PASS=guest rabbitmq:3-management
