### Pet-проект Yatube 
Социальная сеть для публикации дневника.
*Проект построен на классической MVT архитектуре Django. 
Предусмотрена пагинация страниц и кэширование, верификация и регистрация данных, работа с пользователями. 
Написаны тесты для проверки сервиса.*


### Стек технологий
![python version](https://img.shields.io/badge/Python-3.7-yellowgreen) ![django version](https://img.shields.io/badge/Django-2.2-yellowgreen) ![pillow version](https://img.shields.io/badge/Pillow-8.3-yellowgreen) ![pytest version](https://img.shields.io/badge/pytest-6.2-yellowgreen) ![requests version](https://img.shields.io/badge/requests-2.26-yellowgreen) ![sorl-thumbnail version](https://img.shields.io/badge/thumbnail-12.7-yellowgreen)


### Как запустить проект
Клонировать репозиторий и перейти в него в командной строке:

```
https://github.com/DamirShamsutdinov/Yatube_pet-project.git
```

Перейти в папку с проектом

```
cd yatube
```

Cоздать и активировать виртуальное окружение:

```
WIN: python -m venv venv
MAC: python3 -m venv venv
```

```
WIN: source venv/scripts/activate
MAC: source venv/bin/activate
```

Установить зависимости из файла requirements.txt:

```
WIN: python -m pip install --upgrade pip
MAC: python3 -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
WIN: python manage.py migrate
MAC: python3 manage.py migrate
```

Запустить проект:

```
WIN: python manage.py runserver
MAC: python3 manage.py runserver
```

### Набор доступных эндпоинтов:
* ```posts/``` - Отображение постов и публикаций (_GET, POST_);
* ```posts/{id}``` - Получение, изменение, удаление поста с соответствующим **id** (_GET, PUT, PATCH, DELETE_);
* ```posts/{post_id}/comments/``` - Получение комментариев к посту с соответствующим **post_id** и публикация новых комментариев(_GET, POST_);
* ```posts/{post_id}/comments/{id}``` - Получение, изменение, удаление комментария с соответствующим **id** к посту с соответствующим **post_id** (_GET, PUT, PATCH, DELETE_);
* ```posts/groups/``` - Получение описания зарегестрированных сообществ (_GET_);
* ```posts/groups/{id}/``` - Получение описания сообщества с соответствующим **id** (_GET_);
* ```posts/follow/``` - Получение информации о подписках текущего пользователя, создание новой подписки на пользователя (_GET, POST_).<br/>

### Визуализация развернутого проекта:
*http://alvaresshd.pythonanywhere.com/*