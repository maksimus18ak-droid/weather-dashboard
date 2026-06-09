weather-dashboard/
├── flask-app/
│   ├── app.py
│   ├── templates/
│   │   └── index.html
│   └── static/
│       └── style.css
├── react-express-app/
│   ├── backend/
│   │   └── server.js
│   └── frontend/
│       ├── src/
│       │   ├── App.js
│       │   └── index.js
│       └── package.json
├── vue-app/
│   ├── index.html
│   ├── main.js
│   └── style.css
└── README.md
# Weather Dashboard

Веб-приложение для отображения текущей погоды и прогноза на 5 дней с графиком температуры. Реализовано на трёх технологических стеках: Python/Flask, Node.js/Express+React, чистый Vue.js.

## Особенности
- Поиск города с кэшированием (Flask и Express – in-memory, Vue – localStorage не реализован для простоты).
- Отображение температуры, влажности, ветра, описания.
- График изменения температуры (Chart.js).
- Адаптивный дизайн.

## Как запустить

### 1. Flask версия
```bash
cd flask-app
pip install flask requests
# Замените 'your_openweathermap_api_key' в app.py
python app.py
