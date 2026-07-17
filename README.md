# test_api_dmitry_dobrynin

Автотесты для API http://objapi.course.qa-practice.com/object на pytest + requests.
Покрыты методы GET, POST, PUT, PATCH, DELETE.

## Установка

Клонируем репозиторий и переходим в папку (важно, чтобы папка называлась именно
test_api_dmitry_dobrynin — от этого зависят импорты в проекте, при обычном git clone так и будет):

```
git clone <URL_репозитория>
cd test_api_dmitry_dobrynin
```

Ставим виртуальное окружение и зависимости:

```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Запуск тестов

Из корня проекта:

```
pytest
```

Можно запускать по маркеру (critical / medium / minor), например:

```
pytest -m critical
```

## Allure-отчёт

```
pytest --alluredir=allure-results
allure serve allure-results
```
