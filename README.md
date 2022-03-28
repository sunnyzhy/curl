# CURL

## 1 GET

```bash
# curl -X GET http://192.168.0.100:8080/user
```

## 2 POST

```bash
# curl -H "Content-type: application/json" -X POST http://192.168.0.100:8080/user -d '{"id":1,"array":[1,2]}'
```

## 3 DELETE

```bash
# curl -H "Content-type: application/json" -X DELETE http://192.168.0.100:8080/user -d '{"id":1}'
```

## 4 AUTH

```bash
# curl -u name:passwd -X GET http://192.168.0.100:8080/user
```

## 5 添加多个 header

```bash
# curl -H "Content-type: application/json" -H 'header1-: header1' -H 'header-2: header2 -X POST http://192.168.0.100:8080/user -d '{"id":1,"array":[1,2]}'
```

## 6 格式化响应

### 6.1 Python 格式化

```bash
# curl -X GET http://192.168.0.100:8080/user | python -m json.tool

# curl -X GET http://192.168.0.100:8080/user -s | python -m json.tool
```

### 6.2 Nodejs 格式化

```bash
# npm install -g json

# curl -X GET http://192.168.0.100:8080/user | json

# curl -X GET http://192.168.0.100:8080/user -s | json
```

- -s, 不显示 curl 的统计信息

