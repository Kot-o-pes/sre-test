1. Импортировать https://github.com/prometheus/client_python
2. Создать две метрики http_request_total тип counter и http_request_duration тип histogram по 99,95,90 перцентилям 
3. Метрики должны выводится на эндпоинт /metrics 