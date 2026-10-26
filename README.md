# softikna-site

Сайт-портал для Telegram канала [@softikna](https://t.me/softikna)

## Структура проекта
```
softikna-site/
├── app.py              # Flask приложение
├── requirements.txt    # Зависимости
├── Procfile            # Для Render.com
└── templates/
    └── index.html      # Главная страница
```

## Локальный запуск

```bash
pip install flask
python app.py
```
Открыть: http://localhost:5000

## Деплой на Render.com (бесплатно)

1. Загрузи проект на [GitHub](https://github.com)
2. Зарегистрируйся на [render.com](https://render.com)
3. Нажми **New → Web Service**
4. Подключи репозиторий
5. Настройки:
   - **Build Command:** `pip install -r requirements.txt`
   - **Start Command:** `gunicorn app:app`
6. Нажми **Deploy** — сайт будет на `*.onrender.com`
