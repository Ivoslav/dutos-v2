# DUTOS v2 — Система за управление на наряди, отпуски и служебни задължения

### DUTOS — Duty, Leave and Task Organization System

---

## 📝 Описание | Description

**DUTOS v2** е модернизирана уеб система, изградена с **Laravel**, за вътрешна употреба във военно поделение.
Тя осигурява централизирано управление на:

* наряди и графици
* отпуски и командировки
* екипажи, войници и роли
* системни логове и справки

**DUTOS v2** is a modernized Laravel-based web system for internal use in military units, providing centralized management of duties, leaves, assignments, crews, and personnel.

---

## ⚙️ Основни функции | Key Features

* 🔐 Сигурен вход с ролево управление (auth & roles via Laravel)
* 🧏 Управление на потребители, роли и екипажи
* 🗓️ Графици за наряди с възможност за заместване
* ✈️ Отпуски и командировки
* 🧾 Централизирани логове и отчетност
* 📊 Справки и експортиране (предстоящи)

---

## 🧱 Структура на проекта | Project Structure

```
dutos-v2/
├── app/                # Laravel application core
├── database/           # Миграции и seed данни / Migrations & seeds
├── public/             # Публична директория / Public entry point
├── resources/          # Blade templates, Vue/React (future SPA)
├── routes/             # API и web маршрути / Routes
├── storage/            # Логове и файлове / Logs & storage
└── README.md
```

---

## 💾 Изисквания | Requirements

* PHP 8.2+
* Composer
* PostgreSQL 15+
* Laravel 11+
* Node.js & npm (ако ще се ползва Vue/React SPA)

---

## 🚀 Стартиране | Getting Started

1. Клонирай проекта:

   ```bash
   git clone https://github.com/Ivoslav/dutos-v2.git
   cd dutos-v2
   ```

2. Инсталирай зависимостите:

   ```bash
   composer install
   npm install && npm run dev   # само ако имаш frontend assets
   ```

3. Копирай `.env.example` в `.env` и настрой базата:

   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

4. Създай базата и пусни миграциите:

   ```bash
   php artisan migrate --seed
   ```

5. Стартирай вграден сървър:

   ```bash
   php artisan serve
   ```

   После отвори:

   ```
   http://localhost:8000
   ```

---

## 🚰 Планирани подобрения | Upcoming Features

* SPA интерфейс с Vue или React
* PDF/Excel експортиране на справки
* Известия (email + вътрешни)
* Админ панел с разширени настройки
* Интеграция с API за автоматизации

---

## 🛡️ Лиценз | License

Този проект е предназначен за вътрешна употреба и не е публично достъпен без разрешение.
This project is for internal use and not intended for public distribution without permission.

---

**Автор / Author**: [Ivoslav Petkov](https://github.com/Ivoslav)
