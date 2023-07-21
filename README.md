## для server.py
1. Импортировать https://github.com/prometheus/client_python
2. Создать две метрики http_request_total тип counter и http_request_duration тип histogram по 99,95,90 перцентилям 
3. Метрики должны выводится на эндпоинт /metrics 

## для server.go
1. Создать самоподписный сертификат 
```
openssl req -x509 -nodes -days 2 -newkey rsa:2048 -keyout key.pem -out cert.pem
```
2. Импортировать https://pkg.go.dev/github.com/prometheus/client_golang/prometheus/promhttp
3. Создать две метрики http_request_total тип counter и http_request_duration тип histogram по 99,95,90 перцентилям 
4. Добавить метрику https_certificate_expiry_date которая отдает данные о сроке истечения сертификата в формате epoch
5. вывести метрики на /metrics 
