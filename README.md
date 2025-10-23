# 🎓 StudentSystem

Система учёта студентов, курсов и оценок, реализованная на Python (FastAPI + SQLAlchemy + PostgreSQL).

## 📘 Описание проекта
Приложение позволяет:
- Добавлять и редактировать студентов и курсы;
- Назначать студентов на курсы;
- Вносить и обновлять оценки;
- Получать данные через REST API.

## 🧩 Архитектура проекта
Проект построен по многослойной архитектуре:
- **UI/API (FastAPI)** – взаимодействие с пользователем через REST endpoints.
- **BLL (Business Logic Layer)** – бизнес-логика и валидация данных.
- **DAL (Data Access Layer)** – работа с базой данных через ORM (SQLAlchemy).

## 🗃 Структура проекта
```
StudentSystem/
│
├── app/
│   ├── main.py
│   ├── routers/
│   │   ├── students.py
│   │   └── courses.py
│   ├── services/
│   │   ├── student_service.py
│   │   └── course_service.py
│   ├── models/
│   │   ├── student.py
│   │   └── course.py
│   ├── database/
│   │   └── db_connection.py
│   └── schemas/
│       ├── student_schema.py
│       └── course_schema.py
│
├── requirements.txt
├── README.md
└── .gitignore
```

## ⚙️ Технологии
- **Python 3.12**
- **FastAPI**
- **SQLAlchemy**
- **PostgreSQL**
- **PyCharm / VS Code**

## 🚀 Запуск проекта
1. Клонируй репозиторий:
   ```bash
   git clone https://github.com/username/StudentSystem.git
   ```
2. Перейди в директорию проекта:
   ```bash
   cd StudentSystem
   ```
3. Установи зависимости:
   ```bash
   pip install -r requirements.txt
   ```
4. Запусти приложение:
   ```bash
   uvicorn app.main:app --reload
   ```
5. Открой браузер и перейди:
   ```
   http://127.0.0.1:8000/docs
   ```

## 📋 Авторы
- **ФИО студента:** Иванов Иван Иванович  
- **Группа:** ИС-21  
- **Преподаватель:** Петров П.П.
