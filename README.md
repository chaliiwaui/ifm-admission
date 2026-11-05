<p align="center">
  <img src="resources/images/logo.svg" alt="IFM Admission logo" width="96" height="96">
</p>

<h1 align="center">IFM Admission</h1>

<p align="center">
  Laravel 9 admin starter for an admissions portal, built on the Icewall Tailwind CSS admin template.<br>
  Authentication, dashboards, CRUD layouts, calendar, editors and 60+ ready-made pages.
</p>

<p align="center">
  <a href="#-features">✨ Features</a> •
  <a href="#-quick-start">🚀 Quick Start</a> •
  <a href="#-scripts">📦 Scripts</a> •
  <a href="#-structure">🏗️ Structure</a> •
  <a href="#-configuration">⚙️ Configuration</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Laravel-9-FF2D20?logo=laravel&logoColor=white" alt="Laravel 9">
  <img src="https://img.shields.io/badge/PHP-8.0%2B-777BB4?logo=php&logoColor=white" alt="PHP 8">
  <img src="https://img.shields.io/badge/Tailwind-3-06B6D4?logo=tailwindcss&logoColor=white" alt="Tailwind CSS 3">
  <img src="https://img.shields.io/badge/Laravel%20Mix-6-00BFFF" alt="Laravel Mix 6">
  <img src="https://img.shields.io/badge/Icewall-2.0.3-1E40AF" alt="Icewall 2.0.3">
</p>

---

## 🌟 Highlights

- 🧊 **Icewall 2.0.3** – Left4code's Tailwind admin template wired into Laravel with Blade layouts
- 🔐 **Session auth** – login/register flows via `AuthController` with a `loggedin` guard
- 🎨 **Theme switching** – dark mode and five colour schemes persisted in the session
- 🧱 **Three layouts** – side menu, simple menu and top menu, all driven from `app/Main/*Menu.php`

## ✨ Features

- **Dashboards** – four dashboard variants with Chart.js widgets
- **Apps** – inbox, file manager, point of sale, chat, post editor and FullCalendar calendar
- **CRUD & users** – data list / form pages, user and profile layouts, wizard and update-profile screens
- **UI kit** – accordions, modals, slide-overs, notifications (Toastify), tooltips (Tippy), sliders, image zoom, progress bars
- **Forms** – Tom Select, Litepicker date picker, Dropzone uploads, Pristine validation, CKEditor 5 (classic, inline, balloon, balloon-block, document)
- **Tables** – Tabulator data tables with xlsx export
- **Demo data** – `FakerComposer` view composer feeds pages with sample users and images

## 🚀 Quick Start

```bash
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
npm install
npm run dev          # compiles Tailwind (PostCSS) + Mix bundles into public/dist
php artisan serve
```

Register a user at `/register`, then sign in at `/login`.

## 📦 Scripts

| Script               | Description                                              |
| -------------------- | -------------------------------------------------------- |
| `npm run dev`        | Development build                                        |
| `npm run watch`      | Watch Tailwind (`postcss --watch`) and Mix concurrently  |
| `npm run watch-poll` | Mix watch with polling                                   |
| `npm run hot`        | Hot module replacement                                   |
| `npm run prod`       | Production build (PostCSS + `mix --production`)          |

## 🏗️ Structure

```
.
├── app/
│   ├── Http/Controllers/     # AuthController, PageController, DarkMode/ColorScheme switchers
│   ├── Http/View/Composers/  # Menu, dark-mode, colour-scheme, logged-in user, faker composers
│   ├── Main/                 # SideMenu / SimpleMenu / TopMenu definitions
│   └── Models/User.php
├── database/migrations/      # users, password_resets, failed_jobs, personal_access_tokens
├── resources/
│   ├── css/                  # app.css + Tailwind component partials
│   ├── js/                   # One entry per widget (chart, calendar, ckeditor-*, tabulator…)
│   ├── views/layout/         # base, main, side-menu, simple-menu, top-menu, login
│   └── views/pages/          # 64 Blade pages
├── public/dist/              # Compiled assets (committed)
├── routes/web.php            # Auth + page routes
├── tailwind.config.js
├── postcss.config.js
└── webpack.mix.js
```

## ⚙️ Configuration

Environment variables (see `.env.example`): `APP_NAME`, `APP_ENV`, `APP_KEY`, `APP_DEBUG`, `APP_URL`, `LOG_*`, `DB_CONNECTION`, `DB_HOST`, `DB_PORT`, `DB_DATABASE`, `DB_USERNAME`, `DB_PASSWORD`, `BROADCAST_DRIVER`, `CACHE_DRIVER`, `FILESYSTEM_DISK`, `QUEUE_CONNECTION`, `SESSION_DRIVER`, `SESSION_LIFETIME`, `MEMCACHED_HOST`, `REDIS_*`, `MAIL_*`, `AWS_*`, `PUSHER_*`, `MIX_PUSHER_APP_KEY`, `MIX_PUSHER_APP_CLUSTER`.

## 🚀 Deployment

Point the web root at `public/`, run `composer install --no-dev --optimize-autoloader`, `php artisan migrate --force`, `npm run prod`, then cache config and routes.

## 🧪 Testing

```bash
vendor/bin/phpunit
```

## 📄 License

No license has been chosen yet. The Icewall template is © Left4code and subject to its own license.

## 👤 Author

**Jackson Makinda** – [makindajackson.com](https://makindajackson.com)

- 📧 Email: me@makindajackson.com
- 💼 LinkedIn: [Jackson Makinda](https://linkedin.com/in/makindajack)
- 🎨 Dribbble: [@makindajack](https://dribbble.com/makindajack)
- 🐦 Twitter: [@makindajack](https://twitter.com/makindajack)

---

Built with ❤️ in Dar es Salaam, Tanzania 🇹🇿
