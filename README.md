# Simple API written in GO using Gin Framework

## Endpoint test with rest client (VsCode Extension)

```json
# List todos

# List Version
GET http://localhost:9090/version

# List todo by ID
GET http://localhost:9090/todos/3

# Test non existing todo
GET http://localhost:9090/todos/10

# Add new todo
POST http://localhost:9090/todos HTTP/1.1
content-type: application/json

{
"id": "4",
"item": "Cook Meal",
"completed": true
}

# Patch todo
PATCH http://localhost:9090/todos/3
```

## Build and Run

```bash
docker compose -f ./docker-compose.yaml build
docker compose -f ./docker-compose.yaml up
```
