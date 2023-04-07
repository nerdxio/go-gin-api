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
- json response

```json
[
    {
        "id": "1",
        "title": "album1",
        "artist": "artist1",
        "price": 10
    },
    {
        "id": "2",
        "title": "album2",
        "artist": "artist2",
        "price": 20
    }
]
```

-get album by id

```bash
curl -X GET http://localhost:8080/albums/1
```

- json response

```json
{
    "id": "1",
    "title": "album1",
    "artist": "artist1",
    "price": 10
}
```
add new album

```bash
curl -X POST http://localhost:8080/albums -H "Content-Type: application/json" -d '{"id": "3", "title": "new album", "artist": "new artist", "price": 10}'
```

- json response

```json
{
    "id": "3",
    "title": "new album",
    "artist": "new artist",
    "price": 10
}
```