Docker-основа для развертывания среды разработки сайтов на стеке php+mysql.

Docker-compose собирает 3 образа:

1. Основной: nginx+php-fpm (рабочий каталог: текущий)
2. MySQL 5.7 (рабочий каталог `./mysql`)
3. Mailhog для отладки почты

В качестве основы взята структура образов из laravel sail

## Установка

```bash
git clone git@github.com:azernov/dockermodx

cd dockermodx

./lectoria-docker up
```

После успешной сборки будут запущены 3 контейнера

## Подключение к терминалу основного контейнера

```bash
./lectoria-docker shell
```
