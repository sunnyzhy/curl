# CURL

## 1. GET

```bash
# curl -X GET http://192.168.0.100:8080/user
```

## 2. POST

```bash
# curl -H "Content-type: application/json" -X POST http://192.168.0.100:8080/user -d '{"id":1,"array":[1,2]}'
```

## 3. DELETE

```bash
# curl -H "Content-type: application/json" -X DELETE http://192.168.0.100:8080/user -d '{"id":1}'
```

## 4. AUTH

```bash
# curl -u name:passwd -X GET http://192.168.0.100:8080/user
```

## 5. 格式化响应

### Python 格式化

```bash
# curl -X GET http://192.168.0.100:8080/user | python -m json.tool

# curl -X GET http://192.168.0.100:8080/user -s | python -m json.tool
```

### Nodejs 格式化

```bash
# npm install -g json

# curl -X GET http://192.168.0.100:8080/user | json

# curl -X GET http://192.168.0.100:8080/user -s | json
```

- -s, 不显示 curl 的统计信息

