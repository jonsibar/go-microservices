# go-microservices

A Go-based microservices app utilizing Docker, Docker Compose, and GNU Make for containerization, deployment, and task automation. The app includes a frontend for testing stub services such as authentication, logging, and messaging, integrating PostgreSQL, MongoDB, and RabbitMQ, and employing JSON for inter-service communication

project/Makefile
```make
make help
 Commands:
  up             starts all containers in the background without forcing build
  up_build       stops docker-compose (if running), builds all projects and starts docker compose
  down           stop docker compose
  build_broker   builds the broker binary as a linux executable
  build_logger   builds the logger binary as a linux executable
  build_auth     builds the auth binary as a linux executable
  build_mail     builds the mail binary as a linux executable
  build_front    builds the frone end binary
  start          starts the front end
  stop           stop the front end
  help           displays help
