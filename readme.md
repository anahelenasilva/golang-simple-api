# golang-api-tutorial

A simple Golang api for managing books. All data are saved in memory.
Here are the endpoints and how to use them:

## Get all books
```curl
curl http://localhost:8081/books
```

## Get a book by id
```curl
curl http://localhost:8081/books/1
```

## Create a book
```curl
 curl http://localhost:8081/books --include --header "Content-Type: application/json" -d @body.json --request "POST"
```

PS: this will use the file `body.json` to make it easier to test this endpoint

## Checkout a book
```curl
curl http://localhost:8081/checkout\?id\=2 --request "PATCH"
```

## Return a book