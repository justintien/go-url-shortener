# go-url-shortener

A golang URL Shortener with mysql support.  
<!-- Using Bijective conversion between natural numbers (IDs) and short strings -->

## Usage

```sh
docker-compose up --build
```

## Example

```sh
curl -X POST -H "Content-Type:application/json" -d "{\"url\": \"http://www.google.com\"}" http://localhost:3001/shorten
```

Response:

```sh
{"url":"localhost:8081/3"}
```

Redirect

```sh
curl -v localhost:8081/3
```