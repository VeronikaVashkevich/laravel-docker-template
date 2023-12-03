# Запуск проекта

### Подготовка проекта

- Создать в корне проекта папку src
- В консоли выполнить команды

```sh
docker-compose build
docker compose run composer create-project laravel/laravel .
```

### Настройка подключения к базе данных

```
MYSQL_DATABASE=DB_DATABASE из файла .env Laravel
MYSQL_USER=DB_USERNAME из файла .env Laravel
MYSQL_PASSWORD=DB_PASSWORD из файла .env Laravel
```

В файле src/.env 

```
DB_HOST=mysql - название сервиса БД из файла docker-compose.yml
DB_PORT=3306 - порт сервиса БД из файла docker-compose.yml
```

### Запуск проекта

Выполнить в консоли команду 

```
docker-compose up -d
```