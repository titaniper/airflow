from https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html#fetching-docker-compose-yaml

키 생성 후 설정
```
pip install cryptography

# Fernet 키 생성
python -c "from cryptography.fernet import Fernet; print(Fernet.generate_key().decode())"
# Secret 키 생성
python -c "import secrets; print(secrets.token_urlsafe(16))"
```