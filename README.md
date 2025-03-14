# API Yatube

**API Yatube** — это API для социальной сети Yatube. Позволяет управлять публикациями, комментариями, подписками и сообществами.

## Установка и запуск

1. **Клонируйте репозиторий**:
   ```sh
   git clone git@github.com:nastyushaaaa/api_final_yatube.git
   ```

2. **Перейдите в директорию проекта**:
   ```sh
   cd api_final_yatube
   ```

3. **Создайте виртуальное окружение, активация и установка зависимостей**:
   ```sh
   python -m venv venv
   source venv/Scripts/activate
   pip install -r requirements.txt
   ```

4. **Перейдите в django проект**:
   ```sh
   cd yatube_api
   ```

5. **Примените миграции**:
   ```sh
   python manage.py migrate
   ```

6. **Запустите сервер**:
   ```sh
   python manage.py runserver
   ```

## Примеры запросов
### Получение списка постов
```
GET /posts/
```
### Получение публикации по id
```
GET /posts/{{post_id}}/
```
### Добавление комментария
POST /posts/{{post_id}}/comments/
Content-Type: application/json
Authorization: Bearer <your_token>

{
    "text": "Тестовый комментарий"
}

### Документация:
```
http://127.0.0.1:8000/redoc/
```


## Авторы

- Платонова Анастасия
