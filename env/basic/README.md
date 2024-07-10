
키 생성 후 설정
```
pip install cryptography

python -c "from cryptography.fernet import Fernet; print(Fernet.generate_key().decode())"
```