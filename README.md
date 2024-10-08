# Semantic Notes Search

Приложение на основе FastAPI для семантического поиска по текстовым заметкам с использованием современных моделей трансформеров. Проект позволяет пользователям управлять заметками и выполнять семантический поиск по их содержимому.

## Возможности

- Создание, обновление и удаление текстовых заметок
- Генерация семантических эмбеддингов для заметок с использованием модели E5-small-v2
- Выполнение семантического поиска по заметкам
- Визуализация семантических связей между заметками с помощью графов
- RESTful API для всех операций

## Технический стек

![Python 3.8+](https://img.shields.io/badge/Python%203.8%2B-090909?style=flat-square&logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-090909?style=flat-square&logo=fastapi) 
![PyTorch](https://img.shields.io/badge/PyTorch-090909?style=flat-square&logo=pytorch)
![Transformers](https://img.shields.io/badge/Transformers-090909?style=flat-square&logo=Hugging%20Face) 
![scikit-learn](https://img.shields.io/badge/scikit--learn-090909?style=flat-square&logo=scikit-learn) 
![NumPy](https://img.shields.io/badge/numpy-090909?style=flat-square&logo=numpy)


## Установка

1. Клонируйте репозиторий:
    ```bash
    git clone https://github.com//MaximSkutsim/semantic-notes-search.git
    cd semantic-notes-search
    ```

2. Создайте виртуальное окружение и активируйте его:
    ```bash
    python -m venv venv
    source venv/bin/activate  # Для Windows: venv\Scripts\activate
    ```

3. Установите зависимости:
    ```bash
    pip install -r requirements.txt
    ```

## Использование

1. Запустите FastAPI сервер:
    ```bash
    python src/app.py
    ```

2. API будет доступен по адресу `http://localhost:8000`

3. API эндпоинты:
    - POST `/build_embeddings/` - Генерация эмбеддингов для заметок
    - POST `/query_semantic/` - Выполнение семантического поиска


## Структура проекта

- `src/` - Каталог исходного кода
  - `app.py` - FastAPI приложение и эндпоинты
  - `index_file.py` - Функциональность для семантического поиска и эмбеддингов
  - `notes_processing.py` - Операции управления заметками
  - `visualization.py` - Инструменты для визуализации графов
- `tests/` - Тестовые файлы
- `docs/` - Документация
- `examples/` - Скрипты примеров использования

## Лицензия

MIT.
