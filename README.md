# ELK Hello World

```bash
docker-compose up -d


curl -X POST -H "Content-Type: application/json" -d '{"message": "Hello World from Docker ELK!"}' http://localhost:5044

Invoke-RestMethod -Uri "http://localhost:5044" -Method Post -Headers @{"Content-Type"="application/json"} -Body '{"message": "Hello World from Docker ELK!"}'

Invoke-RestMethod -Uri "http://localhost:9200/helloworld-index/_doc" -Method Post -Headers @{"Content-Type"="application/json"} -Body '{"message": "Hello World direct to ES!"}'

```
Kibana

http://localhost:5601  