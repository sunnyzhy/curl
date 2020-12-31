# CURL
## GET
```bash
# curl -X GET http://192.168.0.100:8080/user
```

## POST
```bash
# curl -H "Content-type: application/json" -X POST http://192.168.0.100:8080/user -d '{"id":1,"array":[1,2]}'
```

## DELETE
```bash
# curl -H "Content-type: application/json" -X DELETE http://192.168.0.100:8080/user -d '{"id":1}'
```

## Using Passwords
```bash
# curl -u name:passwd -X GET http://192.168.0.100:8080/user
```
