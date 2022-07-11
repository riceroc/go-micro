# Go-Micro
Go microservices project using a Broker service to handle any front end requests and an authentication service with a Postgres DB for storing users.

## How to Run
| Command | Action |
|-------- | ------ |
`make start` | starts the front end
`make up_build` | build the binaries and docker images using docker compose
`make up` | starts docker compose (use after images have been built)
`make down` | bring down docker compose build
`make stop` | stop the frontend application

### Services and Ports
| Service | Host Port | Container Port
| ---- | --------- | -------------|
Frontend | 8080
Broker-service | 8081 | 80
Authentication-service | 8082 | 80
Postgres | 5432 | 5432
