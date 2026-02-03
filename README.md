# movieKernel

A lightweight Go REST API for managing movies. Built with Gorilla Mux.

## Quick Info
- CRUD operations for movies
- JSON API
- In-memory storage (resets on server restart)

## Endpoints
GET /movies → list all movies
GET /movies/{id} → get movie by ID
POST /movies → create movie
PUT /movies/{id} → update movie
DELETE /movies/{id} → delete movie


## Movie Example
```json
{
  "id": "1",
  "isbn": "438229",
  "title": "ProjectX",
  "director": {
    "firstname": "John",
    "lastname": "Doe"
  }
}
Run
git clone https://github.com/yourusername/movieKernel.git
cd movieKernel
go get github.com/gorilla/mux
go run main.go
Server runs at http://localhost:8000
