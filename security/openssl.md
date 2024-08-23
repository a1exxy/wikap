# Проверка соответствия SSL сертификата и ключа

    openssl x509 -noout -modulus -in /путь/до/сертификата/cert.crt | openssl md5

    openssl rsa -noout -modulus -in /путь/до/ключа/my_key.key | openssl md5

    openssl verify -CAfile ca.crt client.crt