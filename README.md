# sqs-publisher-spring

Run SQS Localstack:

docker-compose up -d
docker exec -it localstack /bin/bash
aws --endpoint-url=http://localhost:4566 sqs create-queue --queue-name sample-queue.fifo --attributes FifoQueue=true
