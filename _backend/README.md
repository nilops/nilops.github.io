This should (eventually) be a golang backend that shoves incoming POST data onto a message bus.  Probably needs some auth or something too.

Requires boot2docker for local testing.

Where boot2docker is running 192.168.59.103

```
docker build -t nilops1 .
docker run -it -p 8080:3000 nilops1
curl http://`boot2docker ip`:8080/ping
```
