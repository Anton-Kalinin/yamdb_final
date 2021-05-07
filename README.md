![badge](https://github.com/Anton-Kalinin/yamdb_final/actions/workflows/yamdb_workflow.yaml/badge.svg)
# API YaMDb
API YaMDb - это база данных фильмов, книг, музыки, и API - сервис для работы с этой базой данных.
## Стэк технолгий
Python 3, Django REST FrameWork, PostgreSQL, Docker.
# Запуск
Для запуска проекта необходимо развернуть несколько контейнеров:
``` docker-compose up ```

Далее следует применить миграции с помощью:
``` docker-compose exec web python manage.py migrate --noinput ```

Потом надо собрать статику комантдой:
``` docker-compose exec web python manage.py collectstatic ```

## Ссылка на развернутый проект
[YaMDb](http://84.201.176.77/api/v1/)