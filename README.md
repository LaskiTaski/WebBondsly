# 📈 Web-Bondsly

**Bondsly** — это веб-приложение на Django + DRF для анализа облигаций (пока только ОФЗ).  
Проект вырос из телеграм-бота и теперь медленно превращается в серьезный инструмент анализа и визуализации, с графиками, фильтрами и авторизацией

---

## 🚀 Стек технологий

- **Backend**: Django, Django REST Framework
- **Frontend**: HTML, Bootstrap 5, Chart.js
- **Парсинг**: BeautifulSoup, Requests
- **База данных**: PostgreSQL (временно SQLite, пока Docker не завезли)
- **Будет позже**: Docker, Celery + RabbitMQ, Redis, тесты, CI/CD и другие страшные вещи

---

<details>
<summary>📁 Структура проекта</summary>

| Путь | Назначение |
|------|------------|
| `backend/analyzer/` | Приложение для облигаций |
| `backend/users/` | Кастомные пользователи |
| `backend/core/` | Middleware и общие утилиты |
| `frontend/` | HTML-шаблоны, Bootstrap, JS |
| `securities_analyzer/settings/` | dev.py, prod.py, base.py — конфиги проекта |
| `securities_analyzer/urls.py` | Главный router |
| `securities_analyzer/wsgi.py`, `asgi.py` | WSGI / ASGI точки входа |
| `.env` | Переменные окружения |
| `manage.py` | Запуск Django-проекта |
| `requirements.txt` | Зависимости проекта |

</details>

## ⚙️ Установка

1. Клонируем проект:
```bash
git clone https://github.com/твоя-мечта/bondsly.git
cd bondsly
```

2. Создаем и активируем виртуальное окружение:
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
```

3. Устанавливаем зависимости:
```bash
pip install -r requirements.txt
```

4. Запускаем миграции:
```bash
python manage.py makemigrations
python manage.py migrate
```

5. Создаем суперпользователя (если надо):
```bash
python manage.py createsuperuser
```

6. Запускаем сервер:
```bash
python manage.py runserver
```

## 📦 API
• GET /api/bonds/ — получить список облигаций

• 🔜 Будет больше: фильтрация, избранное, пользовательские настройки, календарь выплат и всё, что может понадобиться.

## 🧪 Тесты
• pytest - Появятся позже.

## 🧨 TODO
- **Настроить структуру проекта.**
- **Создать базовую модель облигации.**
- **Поднять API.**
- **Вывести график доходности / дюрации.**
- **Авторизация и личные портфели.**
- **Календарь выплат.**
- **Docker + Celery + Redis.**

## 💬 Контакты
Пиши на почту / Telegram / GitHub

## 🧠 Лицензия
MIT. Клонируй, ковыряй, используй — но не забывай писать комментарии в коде.

## 🖼️ Скриншоты (Появятся позже)
