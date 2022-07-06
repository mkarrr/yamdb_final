# api_final

## Описание проекта:
 
Обеспечивает доступ к API ресурса Yamdb.
Проект YaMDb собирает отзывы пользователей на произведения.

## Как запустить проект:

**Клонировать репозиторий и перейти в него в командной строке:**

```
git clone git@github.com:mkarrr/infra_sp2.git
cd infra_sp2
```

**Собрать и запустить контейнеры**
```
docker-compose up -d --build 
```

**Выполнить миграции:**

```
docker-compose exec web python manage.py migrate
```

**Загрузить тестовые данные**

```
docker=compose exec web python manage.py load_data_csv [путь к папке с данными]
```

### URLs проекта

После установки проекта будут доступны следующие разделы:

#### Документация API

```
http://hostname:port/redoc/
```

#### Интерфейс API

```
http://hostname:port/api/v1/
```

#### Админка

```
http://hostname:port/admin/
```

Где hostname - имя хоста с развернутым проектом, port - номер порта.


## Авторы

[@mkarrr](https://github.com/mkarrr)

![yamdb workflow](https://github.com/mkarrr/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)
