# Fuel Accounting System

RESTful вебзастосунок для лабораторної роботи з предметної галузі ІС «Облік пально-мастильних матеріалів». Інтерфейс генерується на сервері через Jinja2, дані зберігаються у SQLite, доступ до БД реалізовано через SQLAlchemy ORM.

## Функціональність

- 4 сутності: `User`, `FuelType`, `FuelItem`, `IssueRecord`
- 2 ролі: `admin`, `user`
- повний CRUD для сутності `FuelItem`
- HTML-інтерфейс і JSON API
- змінена OpenAPI документація

## Запуск

```bash
python -m pip install -r requirements.txt
python -m uvicorn app.main:app --reload
```

Після запуску:

- головна сторінка: `http://127.0.0.1:8000/`
- Swagger UI: `http://127.0.0.1:8000/docs/fuel`
- ReDoc: `http://127.0.0.1:8000/docs/reference`

## Демо-акаунти

- адміністратор: `admin / admin123`
- користувач: `operator / user123`
