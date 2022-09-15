# Инструкция по использованию

1. Скопировать файлы `.env.example` в `.env` и `app/.env.example` в `app/.env`
2. Заполнить все переменные окружения необходимыми значениями.
3. Запустить контейнеры `docker-compose up -d`
4. Заполнить базу данных, открытыми данными об аэропортах - `docker exec -it web-udw-dev python3 manage.py refill_avia_data`
   <br>**Важно!** При запуске команды все данные об аэропортах перезаписываются, следовательно комментарии стираются
5. Использовать api по адресу [0.0.0.0:8000](0.0.0.0:8000)
   <br>**Важно** Если переменная `NGINX_PORT` менялась, то необходимо использовать её значение, вместо 8000
6. API документация расположена по адресу [http://0.0.0.0:8000/api/swagger/](http://0.0.0.0:8000/api/swagger/)
7. Развлекаться :)

### Ссылка на заготовки - https://github.com/Ural-Digital-Weekend/Backend-Snippets

