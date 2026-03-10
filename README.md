# **Chromo Crafts** — 3D-печать на заказ

**Chromo Crafts** — интернет-магазин услуг 3D-печати и продажи расходных материалов.

## Основные возможности
- Печать на заказ с использованием PLA, ABS, PETG, смолы и других материалов  
- Поддержка кастомных 3D-моделей от клиентов  
- Продажа расходных материалов для 3D-принтеров  
- Отслеживание статуса заказа и управление процессом печати  
- Выбор качества и детализации печати  

## Технологический стек
| Компонент | Технология |
|-----------|------------|
| Frontend  | React 18, TypeScript, Vite, Tailwind CSS, React Router |
| Backend   | Python 3.11, Django 4.3, Django REST Framework, Celery для фоновых задач |
| База данных | PostgreSQL 16 |
| Хостинг / сервер | DigitalOcean (Droplet), Nginx, Gunicorn |
| Хранение файлов | AWS S3 для 3D-моделей и медиа файлов |
| Платежи | Stripe API для онлайн-оплаты |
| Аутентификация | Django Allauth для регистрации и OAuth (Google, Telegram) |
| Контейнеризация | Docker, Docker Compose |
| DevOps / CI | GitHub Actions для автоматической сборки и тестов |


## Установка и запуск

### 1. Клонируем репозиторий
```bash
git clone https://github.com/sstr-okkt/chromo-crafts.git
```

### 2. Настраиваем Python окружение
```bash
cd backend
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
pip install -r requirements.txt
```

### 3. Миграции базы данных (для Django)
```bash
python manage.py migrate
```

### 4. Запуск сервера
```bash
python manage.py runserver
```

### 5. Запуск фронтенда
```bash
cd ../frontend
npm install
npm start
```

## Возможное развитие проекта

- Добавление интеграции с галереей 3D-моделей
- Автоматическая генерация стоимости печати по материалу и объёму
