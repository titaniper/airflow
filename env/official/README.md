
curl -LfO '<https://airflow.apache.org/docs/apache-airflow/2.5.1/docker-compose.yaml>'

```
https://velog.io/@sophi_e/Airflow-docker-compose%EB%A1%9C-%EC%97%90%EC%96%B4%ED%94%8C%EB%A1%9C%EC%9A%B0-%EC%84%A4%EC%B9%98%ED%95%98%EA%B8%B0 참고


docker compose up --profile flower up 



http://localhost:5555/
http://localhost:28111
airflow
airflow

````

# 커맨드 실행하기

```
curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.5.1/airflow.sh'
chmod +x airflow.sh
./airflow.sh airflow info
```

# 풀 목록 검색 요청 curl
```
ENDPOINT_URL="http://localhost:28111/"
curl -X GET  \
    --user "airflow:airflow" \
    "${ENDPOINT_URL}/api/v1/pools"
```