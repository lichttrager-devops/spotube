<p align="center">
  <img src="assets/banner.png" alt="Spotube" width="100%" />
</p>

<h1 align="center">🎧 Spotube — Перенеси свои плейлисты стильно</h1>

<p align="center">
  ⚡ Миграция с <b>Spotify</b> в <b>YouTube Music</b> <br>
  🖤 Лёгкий интерфейс, прогресс-бар, никаких заморочек.
</p>

---

## 🚀 Возможности

- 🔁 Перенос плейлистов из Spotify в YouTube Music
- ❤️ Поддержка “Любимых треков”
- 📊 Прогресс-бар и отчёт после завершения
- 🧪 Настраиваемая скорость миграции
- 🪄 Полностью локально, никакой телеметрии
- 🤖 Установщик “как Steam” для Windows

## ⚙️ Установка

### 🪄 Быстрый способ (рекомендуется)

1. Скачай [`installer.ps1`](installer.ps1)
2. Запусти от имени администратора
3. Всё установится автоматически: Git, Python, зависимости
4. Spotube запустится после установки

> 💡 Не требует ручной настройки окружения

---

## 🧑‍🔧 Ручная установка (если предпочитаешь)

```bash
git clone https://github.com/username/spotube.git
cd spotube
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python main.py
```

## 🔑 Как получить заголовки YouTube Music

1. Открой YouTube Music в Firefox
2. Включи любое видео
3. Открой Инструменты разработчика (F12 → вкладка Сеть / Network)
4. Обнови страницу (F5) и найди любой запрос к browse, search или player
5. ПКМ по запросу(Request Header) → нажми на RAW и скопируй всё что там есть → вставь в текстовое поле Spotube
6. Нажми “Сохранить” — готово!
 - 🛑 Google Chrome не подойдёт — используй именно Firefox на Windows

## ❓ Частые вопросы
<details> <summary><strong>Что, если токен Spotify устарел?</strong></summary>

Spotube автоматически обновляет его. Если возникает ошибка 401/403 — просто повтори вход, и всё заработает. </details>

<details> <summary><strong>Нужно ли устанавливать ffmpeg?</strong></summary>

Нет. Загрузка и конвертация треков отключены — Spotube сфокусирован на чистой миграции и минимализме. </details>

<details> <summary><strong>Это приложение собирает мои данные?</strong></summary>

Никакой телеметрии. Всё происходит локально, все ключи и заголовки хранятся только у тебя. </details>

## 🤝 Благодарности
- spotipy — для работы с Spotify API
- ytmusicapi — для интеграции с YouTube Music
- Eel — фронтенд на HTML + Python

## 🧠 Автор
Lichttrager AKA kaklowave(tg: xxsqtk)
