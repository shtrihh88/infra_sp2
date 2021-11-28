# Api для сервиса YAMDB

***

Приложение создано с помощью `django` и `django-rest-framework` с использованием
postgresql в качестве базы данных. Запуск возможен с помощью `docker`.

***

## Установка

***

### 1. Подготовить docker согласно официальной [инструкции](https://docs.docker.com/engine/install/).

### 2. Запуск контейнера

```bash
docker-compose up
```

### 3. Выключение контейнера
```bash
docker-compose down
```


## Использование
#### Создание суперпользователя Django
```bash
docker-compose run web python manage.py createsuperuser
```

#### Пример инициализации стартовых данных:
```bash
docker-compose run web python manage.py loaddata fixtures.json
```


## Основные использованные технологии
* python 3.7
* [django](https://www.djangoproject.com/)
* [drf](https://www.django-rest-framework.org/)
* [posgresql](https://www.postgresql.org/)
* [docker](https://www.docker.com/)

