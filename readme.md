Запуск серверу:

Копіюємо файл оточення

```
cp .env.example .env
```

Завантажуємо docker контейнери 
```
docker-compose up -d
```

Завантажуємо дамп бази данних
```
cat dump.sql | docker-compose exec -T mysql usr/bin/mysql -u root --password=password webdev
```

Відкриваємо в браузері http://127.0.0.1:8080
