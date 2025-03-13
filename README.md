# Бот контент-отдела

## Описание
Этот Telegram-бот позволяет пользователям получать ссылки на книги, полезную информацию, бронировать лекции и управлять своими бронированиями. Бот написан с использованием `aiogram` и `aiosqlite`.

## Функциональность
- Регистрация пользователей в базе данных.
- Просмотр и получение ссылок на книги.
- Доступ к полезной информации (текстовые и PDF-файлы).
- Просмотр доступных лекций и бронирование.
- Управление своими лекциями.

## Установка и запуск
### 1. Клонирование репозитория
```sh
git clone https://github.com/pkomarov53/asyncio-content.git
cd telegram-bot
```

### 2. Установка зависимостей
Создайте виртуальное окружение (по желанию) и установите необходимые зависимости:
```sh
pip install -r requirements.txt
```

### 3. Создание базы данных
Перед запуском бота необходимо инициализировать базу данных:
```sh
python -c 'import asyncio; from bot import init_db; asyncio.run(init_db())'
```

### 4. Запуск бота
```sh
python bot.py
```

## Конфигурация
Файл `bot.py` содержит токен бота, который необходимо заменить на ваш в переменной `TOKEN`.

## Структура проекта
```
.
├── bot.py                 # Основной код бота
├── requirements.txt       # Список зависимостей
├── db/                    # Папка для базы данных
├── books/                 # Файлы со ссылками на книги
├── useful_info/           # Полезная информация (тексты, PDF)
├── lections/              # Доступные лекции
└── README.md              # Документация
```

## Используемые технологии
- `aiogram` — асинхронный фреймворк для Telegram-ботов.
- `aiosqlite` — асинхронная работа с SQLite.
- `asyncio` — управление асинхронными задачами.

## Лицензия
Этот проект распространяется под лицензией MIT. Используйте на своё усмотрение!

