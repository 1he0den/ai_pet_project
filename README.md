# 🧐 AI Recipes Generator(Генератор рецептов)

**AI Recipes Generator** — это веб-приложение для генерации и поиска рецептов на основе искусственного интеллекта и внешних API (Spoonacular).

Проект состоит из двух частей:
- **Backend**: FastAPI-сервер для работы с AI и API.
- **Frontend**: React-приложение для взаимодействия с юзером.

---
**ПРИМЕР ИСПОЛЬЗОВАНИЯ**
![image](https://github.com/user-attachments/assets/43cdd56b-4c7d-4db4-9a80-bf5c4964d473)
![image](https://github.com/user-attachments/assets/f3f53452-0f5e-4a0f-9ce4-bc4547ee2ee5)
![image](https://github.com/user-attachments/assets/0c1cebeb-ad47-4fbc-bf49-9f9c7b9047db)


## 📂 Структура проекта

```bash
ai_pet_project/
├── backend/
│   ├— app/
│   │    ├— models/        # Схемы данных
│   │    ├— routers/       # API-роуты
│   │    ├— services/      # Сервисы AI и API
│   │    └— utils/         # Конфиги и зависимости
│   ├— .env             # Переменные окружения
│   ├— requirements.txt # Python-зависимости
│   └— main.py          # Точка входа в backend
│
├── recipe-frontend/
│   ├— src/
│   │    ├— components/  # React-компоненты
│   │    ├— pages/       # Страницы
│   │    └— App.jsx, main.jsx, styles.css
│   ├— package.json   # Node.js зависимости
│   └— vite.config.js (optional)
```

---

# ⚙️ Установка и запуск

## Backend

### 📋 Требования
- Python 3.11+
- pip

### ⚡ Установка
```bash
cd backend
python -m venv venv

# Windows
venv\Scripts\activate

# macOS/Linux
source venv/bin/activate

pip install -r requirements.txt
```

### ⚡ Запуск
```bash
uvicorn app.main:app --reload
```

Доступно на: [http://127.0.0.1:8000](http://127.0.0.1:8000)


## Frontend

### 📋 Требования
- Node.js 18+
- npm или yarn

### ⚡ Установка
```bash
cd recipe-frontend
npm install
```

### ⚡ Запуск
```bash
npm run dev
```

Доступно на: [http://127.0.0.1:5173](http://127.0.0.1:5173)

---

# 🔧 Настройка окружения

В `backend/.env` должны быть заданы API-ключи:

```env
SPOONACULAR_API_KEY=your_spoonacular_api_key
OPENAI_API_KEY=your_openai_api_key
```

---

# 🌏 API Эндпоинты

- `POST /recipes/ai-generate` — Генерация рецепта с помощью AI
- `GET /recipes/search` — Поиск рецептов через Spoonacular API

---

# 🛠️ Стек

- **FastAPI**
- **React 19 + Vite**
- **Ant Design**
- **React Query**
- **OpenAI API**
- **Spoonacular API**

---

# 📌 TODO

- [ ] Дополнить описание API
- [ ] Добавить Docker-файлы
- [ ] Реализовать CI/CD пипелайн
- [ ] Написать unit-тесты

