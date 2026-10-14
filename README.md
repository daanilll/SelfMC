<div align="center">

<img src="docs/logo.png" alt="SelfMC" width="128" height="128">

# SelfMC

**Современный лаунчер Minecraft для Windows с мод-менеджером, автообновлением и приятным интерфейсом**

[![Version](https://img.shields.io/badge/version-6.0.1-8b5cf6?style=for-the-badge)](https://github.com/daanilll/SelfMC/releases)
[![License](https://img.shields.io/badge/license-MIT-10b981?style=for-the-badge)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.12+-3b82f6?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Platform](https://img.shields.io/badge/platform-Windows-f59e0b?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/daanilll/SelfMC/releases)

[![GitHub Stars](https://img.shields.io/github/stars/daanilll/SelfMC?style=for-the-badge&color=fbbf24)](https://github.com/daanilll/SelfMC/stargazers)
[![GitHub Issues](https://img.shields.io/github/issues/daanilll/SelfMC?style=for-the-badge&color=ef4444)](https://github.com/daanilll/SelfMC/issues)
[![Downloads](https://img.shields.io/github/downloads/daanilll/SelfMC/total?style=for-the-badge&color=22c55e)](https://github.com/daanilll/SelfMC/releases)

[🚀 Установка](#-установка) • [✨ Возможности](#-возможности) • [📸 Скриншоты](#-скриншоты) • [🛠 Разработка](#-разработка) • [📄 Лицензия](#-лицензия)

</div>

---

## 🎯 Что такое SelfMC?

**SelfMC** — это красивый и лёгкий лаунчер Minecraft для Windows, написанный на Python с использованием **CustomTkinter**. Он создан для тех, кто устал от громоздких решений и хочет получить всё необходимое в одном месте: установку модов в один клик, управление серверами, автоматические обновления и приятный глазу интерфейс.

> 💡 **Почему SelfMC?** Потому что остальные лаунчеры либо перегружены, либо не работают на Windows «из коробки». SelfMC — лёгкий, нативный, и делает ровно то, что нужно.

---

## ✨ Возможности

### 🎨 Интерфейс
- 🌌 Современная тёмная и светлая темы (переключаются в настройках)
- ✨ Плавные анимации и скруглённые элементы
- 🖼 Кастомная иконка и фон
- 🎯 Нативная интеграция с Windows
- 🌐 Двуязычный интерфейс (RU / EN)

### ⚙️ Управление версиями
- 🚀 Установка **Fabric / Forge / NeoForge / Quilt**
- ☕ Автоматическая загрузка **Java Runtime**
- 📋 Список всех установленных версий
- 🔍 Умный поиск и сортировка версий

### 📦 Моды
- 📦 **Мод-менеджер** с поиском и включением/выключением
- 🔍 Поиск модов на **Modrinth** и **CurseForge**
- 🗂 Сортировка модов по версии Minecraft
- 🎯 **Drag & Drop** модов, ресурспаков и шейдеров
- ➕ Установка **Fabric API** в один клик

### 🔧 Технические
- 🔄 **Автообновление** через GitHub Releases
- 🛡 Умная обработка ошибок
- 🌍 Поддержка зеркала **BMCLAPI** для СНГ
- ⚙️ Прокси для обхода блокировок
- 🎮 **Discord Rich Presence** (статус в Discord)

---

## 📸 Скриншоты

<div align="center">

### 🖥 Главное окно
![Main Window](docs/screenshots/main.png)

### 📦 Мод-менеджер
![Mod Manager](docs/screenshots/mods.png)

### 🔍 Поиск модов
![Mod Search](docs/screenshots/search.png)

### ⚙️ Настройки
![Settings](docs/screenshots/settings.png)

</div>

---

## 🚀 Установка

### 🪟 Windows (10/11)

1. Скачай **`SelfMC-Setup-6.0.1-x64.exe`** из [последнего релиза](https://github.com/daanilll/SelfMC/releases/latest).
2. Запусти установщик.
3. Следуй инструкциям мастера установки.
4. После установки — запусти **SelfMC** из меню «Пуск» или с рабочего стола.

**Требования:**
- Windows 10/11 (64-bit)
- 4 ГБ RAM (рекомендуется 8 ГБ+)

**Примечание:** Windows SmartScreen может показать предупреждение при первом запуске — это нормально для новых программ. Нажми «Подробнее» → «Всё равно запустить».

### 🛠 Установка из исходников

bash
# Установи зависимости (нужен Python 3.12)
pip install customtkinter pillow requests minecraft_launcher_lib tkinterdnd2 pypresence

# Запусти
python main_ctk.py
📋 Требования
Компонент	Минимум	Рекомендуется
ОС	Windows 10 (64-bit)	Windows 11
Python	3.10	3.12+
RAM	4 ГБ	8 ГБ+
Место на диске	2 ГБ	10 ГБ+ (с модами)
🎮 Как пользоваться
1️⃣ Выбор версии
Открой SelfMC → выбери версию в выпадающем списке (например, 1.21.4).

2️⃣ Установка модлоадера
Выбери Fabric / Forge / NeoForge / Quilt → нажми «⤓ Установить».

3️⃣ Установка модов
Из Modrinth: кнопка «🔍 Найти мод» → введи название → «⤓ Установить»

Локально: перетащи .jar прямо в окно SelfMC

Вручную: положи .jar в %APPDATA%\.minecraft\mods\

4️⃣ Запуск
Жми большую зелёную кнопку «▶ ИГРАТЬ».

🛠 Разработка
Структура проекта
text
SelfMC/
├── main_ctk.py              # Основной файл лаунчера
├── installer.py             # Скрипт установщика
├── discord_rpc.py           # Discord Rich Presence
├── black.ico                # Иконка приложения
├── image.jpg                # Фоновое изображение
├── installer.iss            # Inno Setup скрипт
├── build.bat                # Скрипт сборки
├── get_version.py           # Чтение версии из кода
├── VERSION.txt              # Кэш версии для сборки
├── docs/
│   ├── logo.png
│   └── screenshots/
└── README.md
Сборка .exe и установщика
bash
# Просто запусти build.bat
build.bat
Скрипт автоматически:

Прочитает версию из main_ctk.py

Соберёт SelfMC.exe через PyInstaller

Создаст установщик через Inno Setup

Результат появится в installer_output\

Версионирование
Мелкая правка: 6.0.1 → 6.0.2 … 6.0.9

Крупное обновление: 6.0.9 → 6.9.0

Следующий мажор: 6.9.9 → 7.0.0

🤝 Вклад
🐛 Нашёл баг? → Создай Issue

💡 Есть идея? → Открой обсуждение

📝 Pull Request — приветствуется

🗺 Дорожная карта
☑ Базовый функционал
☑ Установка Fabric / Forge / Quilt
☑ Мод-менеджер
☑ Поиск модов
☑ Переход на Windows
☑ Автообновление через GitHub Releases
☑ Discord Rich Presence
□ Менеджер модпаков (Modrinth Modpacks)
□ Менеджер аккаунтов со скинами
□ Поддержка CurseForge
□ Переключатель языка RU / EN
□ Сборка для Linux (.deb / .rpm)
❓ FAQ
<details> <summary><b>SelfMC не запускается, что делать?</b></summary>
Убедись, что установлен Python 3.12 (не 3.15). Если запускаешь из исходников:

bash
python -c "import customtkinter, PIL, requests"
Если что-то падает — установи:

bash
pip install customtkinter pillow requests minecraft_launcher_lib tkinterdnd2 pypresence
</details><details> <summary><b>Как обновить SelfMC?</b></summary>
Запусти — он сам проверит обновления. Или нажми 🔄 в топбаре.

</details><details> <summary><b>Где хранятся настройки и логи?</b></summary>
Настройки: %APPDATA%\SelfMC\settings.json

Лог: %APPDATA%\SelfMC\last_run.log

Игра: %APPDATA%\.minecraft\

</details><details> <summary><b>Как включить/выключить Discord RPC?</b></summary>
Открой Настройки → Лаунчер → галочка «Показывать статус в Discord».

</details><details> <summary><b>Работает ли на Linux?</b></summary>
Пока нет. Проект ориентирован на Windows. В планах — сборка для Linux.

</details><details> <summary><b>Что с CurseForge?</b></summary>
Поддержка CurseForge через API — в разработке.

</details>
📄 Лицензия
Этот проект распространяется под лицензией MIT. Подробности в файле LICENSE.

💖 Благодарности
🎮 Mojang — за Minecraft

🧵 Fabric / Forge / Quilt — за модлоадеры

📦 Modrinth — за открытое API

🐍 Python + CustomTkinter — за инструменты

🎨 Сообщество — за поддержку

<div align="center">
🌟 Понравился проект? Поставь звезду!
https://api.star-history.com/svg?repos=daanilll/SelfMC&type=Date

Сделано с ❤️ на Windows

</div>
