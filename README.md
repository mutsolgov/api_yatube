# **api_yatube**
api_yatube



- `api/v1/api-token-auth/` (POST): передаём логин и пароль, получаем токен.
- `api/v1/posts/` (GET, POST): получаем список всех постов или создаём новый пост.
- `api/v1/posts/{post_id}/` (GET, PUT, PATCH, DELETE): получаем, редактируем или удаляем пост по id.
- `api/v1/groups/` (GET): получаем список всех групп.
- `api/v1/groups/{group_id}/` (GET): получаем информацию о группе по id.
- `api/v1/posts/{post_id}/comments/` (GET, POST): получаем список всех комментариев поста с id=post_id или создаём новый, указав id поста, который хотим прокомментировать.
- `api/v1/posts/{post_id}/comments/`{comment_id}/ (GET, PUT, PATCH, DELETE): получаем, редактируем или удаляем комментарий по id у поста с id=post_id.
___


### Установка и настройки
___

#### *Клонируем проект:*
```python
git clone git@github.com:mutsolgov/api_yatube.git
```

#### *Переходим в папку с ботом.*
```
cd api_yatube
```


*Создаем виртуальное окружение:*
```
python -m venv venv
```

*Запускаем виртуальное окружение:<br>*
```
source venv/Scripts/activate 
``` 

*Устанавливаем зависимости:<br>*
```
python -m pip install --upgrade pip
pip install -r requirements.txt
```

*Выполняем миграции:*
```
python manage.py makemigrations
python manage.py migrate
```

Создаем суперпользователя:
```
python manage.py createsuperuser
```

*Запускаем проект.*
```
python manage.py runserver
```

### *Автор:<br>*
### *Муцольгов Магомед 2023 год.*

