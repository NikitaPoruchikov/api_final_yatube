# API Yatube

API Yatube — это веб-сервис для публикации личных дневников, позволяющий пользователям создавать, просматривать и комментировать посты. Основан на Django и Django REST Framework.

## Начало работы

Эти инструкции помогут вам получить копию проекта на вашем локальном компьютере для разработки и тестирования.

### Предварительные требования

Для запуска этого проекта вам понадобятся следующие инструменты:

- Python (версия 3.8 или выше)
- Django (версия 3.2 или выше)
- Django REST Framework

Вы можете установить все необходимые зависимости через pip:

```bash
pip install django djangorestframework

Установка

Следуйте этим шагам для настройки проекта локально:

	1.	Клонируйте репозиторий:

    git clone https://github.com/your-username/yatube-api.git
    cd yatube-api

    2.	Установите зависимости из файла requirements.txt:

    pip install -r requirements.txt

    3.  Примените миграции:

    python manage.py migrate

    4.  Запустите сервер разработки:

    python manage.py runserver

    Использование

    Примеры использования API:

	•	Получение списка всех постов:

    GET /api/posts/

    •	Добавление нового поста:

    POST /api/posts/
    Content-Type: application/json

    {
    "title": "Название поста",
    "body": "Текст поста",
    "author": "username"
    }