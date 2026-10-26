# PC Sim News — Официальный сайт сообщества

Сайт для интернет-сообщества по игре PC Simulator.

## 📁 Структура проекта

```
pcsite/
├── index.html           # Главная страница
├── assets/
│   ├── gallery/         # 6 изображений галереи
│   ├── artem.png        # Персонаж Артем
│   ├── qr_*.png         # QR-коды каналов
│   └── img_*.webp       # Остальные изображения
├── .nojekyll            # Для GitHub Pages
└── CNAME                # Кастомный домен
```

## 🚀 Деплой на GitHub Pages

### Шаг 1: Создайте репозиторий на GitHub
1. Перейдите на https://github.com/new
2. Укажите имя: `ваш-логин.github.io` (или любое другое)
3. Выберите Public
4. Нажмите "Create repository"

### Шаг 2: Загрузите файлы (через git)
```bash
# Клонировать репозиторий
git clone https://github.com/ваш-логин/ваш-репозиторий.git
cd ваш-репозиторий

# Скопировать файлы сайта
cp -r /mnt/virt/pcsite/* .

# Добавить и отправить
git add .
git commit -m "PC Sim News website"
git push origin main
```

### Шаг 3: Настроить GitHub Pages
1. В репозитории: Settings → Pages
2. Branch: main, папка: / (root)
3. Сохранить

### Шаг 4: Кастомный домен (опционально)
В файле `CNAME` укажите:
```
pcsimnews.work.gd
```
Затем в настройках домена добавьте CNAME запись:
```
pcsimnews.work.gd → ваш-логин.github.io
```

## 🌐 Локальный запуск

```bash
cd /mnt/virt/pcsite
python3 -m http.server 8080
```
Открыть: http://localhost:8080

## 📊 Разделы сайта

- **Главная** — приветствие и слоган
- **Почему мы** — 6 преимуществ сообщества
- **Артем** — маскот с характеристиками
- **Новости** — ссылка на коммьюнити
- **PCS-DOS** — описание DOS-системы
- **Галерея** — 6 изображений из игры
- **Каналы** — QR-коды и ссылки на Telegram

## 📱 Каналы

| Канал | Ссылка | QR-код |
|-------|--------|--------|
| Proovs | https://t.me/pruvipcsimnews | qr_pruvipcsimnews.png |
| Сообщество | https://t.me/pcsimnewscomunity | qr_pcsimnewscomunity.png |
| Email | pcsimnews.commercial.531@mail.ru | qr_email.png |