# Проверка соответствия SSL сертификата и ключа

    openssl x509 -noout -modulus -in /путь/до/сертификата/cert.crt | openssl md5

    openssl rsa -noout -modulus -in /путь/до/ключа/my_key.key | openssl md5

    openssl verify -CAfile ca.crt client.crt

    Проверка соответствия ключа сертификату:


**Отпечатки сертификатов:**

    openssl x509 -in cert.crt -noout -fingerprint

    openssl x509 -in cert.crt -noout -fingerprint -sha256

**Создание самоподписанного сертификата**
    
    openssl req -x509 -newkey rsa:2048 -keyout selfsign.key -out selfsign.crt -days 365 -nodes -subj "/CN=example.com"
