# go-gin-api
Simple API with Golang and Gin framework

### Getting Started

1- clone the repo

```bash
git clone https://github.com/hassanrefaat9/go-gin-api
```

2- add gin dependency

```bash
go get -u github.com/gin-gonic/gin
```
or
you can added to import section in your code

```go
import "github.com/gin-gonic/gin"
```

### Endpoints

- get all albums

```bash
curl -X GET http://localhost:8080/albums
```

-get album by id

```bash
curl -X GET http://localhost:8080/albums/1
```

add new album

```bash
curl -X POST http://localhost:8080/albums -H "Content-Type: application/json" -d '{"id": "3", "title": "new album", "artist": "new artist", "price": 10}'
```