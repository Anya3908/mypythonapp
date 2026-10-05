# my-python-app

Учебный проект с CI на GitHub Actions.

## Что делает CI

- Линтинг (flake8)
- Тесты (pytest) на Python 3.9, 3.10, 3.11, 3.12
- Сборка Docker-образа (без публикации)

## Запуск локально

```bash
pip install -r requirements.txt
pip install -e .
pytest tests/
```

## Docker

```bash
docker build -t my-python-app:test .
docker run --rm my-python-app:test
```