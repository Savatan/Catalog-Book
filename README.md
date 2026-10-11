# Каталог книг

Веб-приложение на Django для просмотра каталога книг, авторов и отзывов.

## Возможности

- Просмотр списка книг.
- Фильтрация каталога по жанрам.
- Сортировка по цене, рейтингу, названию и году издания.
- Страница с подробной информацией о книге и отзывами.
- Отдельная страница со списком авторов.
- Django Admin для управления данными.

## Модель данных

- **Book** — название, автор, жанры, описание, год издания, количество страниц, цена, рейтинг и наличие.
- **Author** — имя, фамилия, год рождения и биография.
- **Genre** — название и slug жанра.
- **Review** — оценка и текст отзыва о книге.

## Технологии

- Python
- Django
- SQLite
- HTML и Django Templates

## Запуск локально

Требуется установленный Python.

```bash
git clone https://github.com/Savatan/Catalog-Book.git
cd Catalog-Book
python -m venv .venv
```

Активируйте виртуальное окружение:

```bash
# macOS / Linux
source .venv/bin/activate

# Windows PowerShell
.venv\\Scripts\\Activate.ps1
```

Установите Django и подготовьте базу:

```bash
python -m pip install django
python manage.py migrate
python seed_data.py
python manage.py runserver
```

Откройте <http://127.0.0.1:8000/>.
