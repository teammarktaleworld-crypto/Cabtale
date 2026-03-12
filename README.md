<p align="center">
  <img src="https://github.com/user-attachments/assets/5f644bd7-3f35-4729-8409-6b13ec49b009" alt="Cabtale Logo" width="320"/>
</p>

<h1 align="center">Cabtale</h1>

<p align="center">
  <em>Connecting riders and drivers with real-time precision.</em>
</p>

<p align="center">
  <a href="https://www.php.net/releases/8.1/en.php"><img src="https://img.shields.io/badge/PHP-8.1%2B-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP 8.1+"/></a>
  <a href="https://laravel.com/docs/10.x"><img src="https://img.shields.io/badge/Laravel-10.x-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel 10"/></a>
  <a href="https://flutter.dev/"><img src="https://img.shields.io/badge/Flutter-3.x-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter 3"/></a>
  <a href="https://dart.dev/"><img src="https://img.shields.io/badge/Dart-3.x-0175C2?style=for-the-badge&logo=dart&logoColor=white" alt="Dart 3"/></a>
  <img src="https://img.shields.io/badge/License-Proprietary-red?style=for-the-badge" alt="License"/>
  <img src="https://img.shields.io/badge/Status-Production%20Ready-brightgreen?style=for-the-badge" alt="Production Ready"/>
</p>

---

## 📑 Table of Contents

- [About Cabtale](#-about-cabtale)
- [Tech Stack](#-tech-stack)
- [Architecture Overview](#-architecture-overview)
- [Key Features](#-key-features)
- [Module Architecture](#-module-architecture)
- [Payment Gateways](#-payment-gateways)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Backend Setup (Laravel)](#backend-setup-laravel)
  - [Flutter Apps Setup](#flutter-apps-setup)
- [Environment Configuration](#-environment-configuration)
- [API Overview](#-api-overview)
- [Real-time Services](#-real-time-services)
- [Security](#-security)
- [Deployment](#-deployment)
- [Project Structure](#-project-structure)
- [Contributing](#-contributing)
- [Copyright](#-copyright)

---

## 🚖 About Cabtale

**Cabtale** is an enterprise-grade, full-stack ride-sharing platform built for speed, reliability, and scale. It ships as three integrated products:

| Product | Description | Technology |
|---|---|---|
| **Backend API** | RESTful API server powering all mobile apps | Laravel 10 · PHP 8.1+ |
| **Cabtale User App** | Passenger-facing mobile application | Flutter · Dart |
| **Cabtale Driver App** | Driver-facing mobile application | Flutter · Dart |

The platform supports trip booking, real-time driver tracking, multi-currency payments, in-app chat, parcel delivery, promotional campaigns, and a full admin panel — all out of the box.

---

## 🛠 Tech Stack

### Backend

<p>
  <img src="https://img.shields.io/badge/PHP-8.1+-777BB4?style=flat-square&logo=php&logoColor=white" alt="PHP"/>
  <img src="https://img.shields.io/badge/Laravel-10.x-FF2D20?style=flat-square&logo=laravel&logoColor=white" alt="Laravel"/>
  <img src="https://img.shields.io/badge/MySQL-8.x-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL"/>
  <img src="https://img.shields.io/badge/Redis-7.x-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
  <img src="https://img.shields.io/badge/Reverb-WebSockets-6C63FF?style=flat-square&logo=laravel&logoColor=white" alt="Laravel Reverb"/>
  <img src="https://img.shields.io/badge/Pusher-Channels-300D4F?style=flat-square&logo=pusher&logoColor=white" alt="Pusher"/>
  <img src="https://img.shields.io/badge/Passport-OAuth2-FF2D20?style=flat-square&logo=laravel&logoColor=white" alt="Laravel Passport"/>
  <img src="https://img.shields.io/badge/Sanctum-API%20Tokens-FF2D20?style=flat-square&logo=laravel&logoColor=white" alt="Laravel Sanctum"/>
</p>

### Mobile

<p>
  <img src="https://img.shields.io/badge/Flutter-3.x-02569B?style=flat-square&logo=flutter&logoColor=white" alt="Flutter"/>
  <img src="https://img.shields.io/badge/Dart-3.x-0175C2?style=flat-square&logo=dart&logoColor=white" alt="Dart"/>
  <img src="https://img.shields.io/badge/GetX-State%20Management-9B59B6?style=flat-square&logo=flutter&logoColor=white" alt="GetX"/>
  <img src="https://img.shields.io/badge/Firebase-Cloud%20Messaging-FFCA28?style=flat-square&logo=firebase&logoColor=black" alt="Firebase FCM"/>
  <img src="https://img.shields.io/badge/Google%20Maps-SDK-4285F4?style=flat-square&logo=googlemaps&logoColor=white" alt="Google Maps"/>
</p>

### Cloud & DevOps

<p>
  <img src="https://img.shields.io/badge/GCP-Cloud%20Platform-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="GCP"/>
  <img src="https://img.shields.io/badge/Firebase-Crashlytics-FFCA28?style=flat-square&logo=firebase&logoColor=black" alt="Firebase"/>
  <img src="https://img.shields.io/badge/Twilio-SMS%20%26%20Voice-F22F46?style=flat-square&logo=twilio&logoColor=white" alt="Twilio"/>
  <img src="https://img.shields.io/badge/Stripe-Payments-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe"/>
</p>

### Full Technology Reference

| Layer | Technology | Version |
|---|---|---|
| Backend Framework | Laravel | 10.10 |
| Server Language | PHP | 8.1+ |
| Primary Database | MySQL | 8.x |
| Caching Layer | Redis | 7.x |
| Real-time Broadcasting | Laravel Reverb | @beta |
| WebSocket Server | Ratchet | 0.4.4 |
| Push Notifications (Web/Server) | Pusher PHP SDK | 7.2 |
| Authentication (OAuth2) | Laravel Passport | — |
| API Token Auth | Laravel Sanctum | 3.3 |
| Module System | nwidart/laravel-modules | 11.0 |
| Geolocation (Spatial) | laravel-eloquent-spatial | 4.0 |
| PDF Generation | DomPDF / mPDF | 2.0 / 8.2 |
| Excel Export | Fast Excel | 5.3 |
| SMS / Voice | Twilio SDK | 7.14 |
| Mobile Framework | Flutter | SDK ≥3.3.0 |
| Mobile Language | Dart | 3.x |
| State Management | GetX | 4.6.6 |
| Mobile Maps | Google Maps Flutter | 2.7.0 |
| Push Notifications (Mobile) | Firebase Cloud Messaging | 16.1.1 |
| Crash Reporting | Firebase Crashlytics | 5.0.7 |
| Cloud Platform | Google Cloud Platform | — |
| Build System | Laravel Mix | 6.0.6 |

---

## 🏗 Architecture Overview

```
┌──────────────────────────────────────────────────────────┐
│                     Cabtale Platform                     │
├───────────────────┬──────────────────┬───────────────────┤
│  Cabtale User App │ Cabtale Driver   │   Admin Panel     │
│  (Flutter/Dart)   │ App (Flutter)    │   (Web/Laravel)   │
└────────┬──────────┴────────┬─────────┴────────┬──────────┘
         │                   │                   │
         └───────────────────┼───────────────────┘
                             │  HTTPS / REST API
                    ┌────────▼────────┐
                    │  Laravel 10 API │
                    │  (public_html/) │
                    └────────┬────────┘
          ┌──────────────────┼─────────────────┐
          │                  │                  │
   ┌──────▼──────┐  ┌────────▼───────┐  ┌──────▼──────┐
   │   MySQL 8   │  │   Redis Cache  │  │ Laravel     │
   │  (Primary   │  │  (Sessions,    │  │ Reverb /    │
   │  Database)  │  │   Queues,      │  │ Pusher WS   │
   └─────────────┘  │   Broadcast)   │  └─────────────┘
                    └────────────────┘
                             │
              ┌──────────────┼──────────────┐
              │              │              │
       ┌──────▼──────┐ ┌─────▼─────┐ ┌─────▼──────┐
       │  Firebase   │ │  Google   │ │  Twilio    │
       │  (FCM/Crash)│ │  Maps API │ │  (SMS)     │
       └─────────────┘ └───────────┘ └────────────┘
```

---

## ✨ Key Features

### 🧑‍💼 Customer App
- **Registration & Authentication** — OTP login, social login (Google/Apple), email/password
- **Ride Booking** — Instant booking, scheduled rides, fare estimation before booking
- **Live Tracking** — Real-time driver location on Google Maps
- **Multiple Stop Support** — Add intermediate stops to a trip
- **Parcel Delivery** — Send packages with live tracking
- **In-App Chat** — Real-time messaging with assigned driver
- **Ratings & Reviews** — Rate drivers and trips after completion
- **Push Notifications** — Trip updates, offers, and alerts via FCM
- **Promotions & Coupons** — Apply discount codes at checkout
- **Wallet & Transactions** — View earnings, add funds, withdraw
- **Multi-Language Support** — Localization ready
- **Dark / Light Theme** — Full theme support

### 🚗 Driver App
- **Registration & Document Verification** — Upload vehicle docs, driving licence
- **Online / Offline Toggle** — Drivers control their availability
- **Trip Requests** — Accept, reject, or bid on ride requests
- **Navigation Integration** — Turn-by-turn navigation support
- **Earnings Dashboard** — Daily/weekly/monthly earnings summary
- **Withdrawal Management** — Request payout to bank/wallet
- **Trip History** — Full history with fare breakdown
- **In-App Chat** — Communicate with passengers
- **Push Notifications** — New ride alerts, promotional messages
- **Parcel Delivery Mode** — Accept parcel delivery requests

### 🛡 Admin Panel
- **Dashboard Analytics** — Revenue, trips, active drivers at a glance
- **User & Driver Management** — CRUD, verification status, account control
- **Vehicle & Category Management** — Define vehicle types and categories
- **Zone Management** — Define service areas geographically
- **Fare Management** — Configure base fare, per-km/minute rates, surge pricing
- **Promotion Management** — Create and manage discount campaigns
- **Payment Gateway Configuration** — Enable/disable gateways per region
- **Transaction Reports** — Export CSV/Excel/PDF financial reports
- **Notification Management** — Send push/SMS/email to users or drivers
- **System Settings** — Control all app behavior from admin panel

---

## 🧩 Module Architecture

Cabtale's Laravel backend uses a modular architecture (via `nwidart/laravel-modules`), keeping each business domain isolated and independently maintainable.

```
public_html/Modules/
├── 📦 AdminModule            — Admin panel controllers & views
├── 🔐 AuthManagement         — Registration, login, OTP, social auth
├── ⚙️  BusinessManagement     — App settings, pages, configurations
├── 💬 ChattingManagement     — Real-time in-app messaging
├── 💰 FareManagement         — Pricing rules, surge, bidding
├── 💳 Gateways               — Payment gateway integrations
├── 📦 ParcelManagement       — Parcel/cargo delivery logic
├── 🏷️  PromotionManagement    — Coupons, referrals, campaigns
├── ⭐ ReviewModule            — Ratings & reviews system
├── 🏦 TransactionManagement  — Wallet, withdrawals, ledger
├── 🚕 TripManagement         — Core trip lifecycle (booking → completion)
├── 👤 UserManagement         — User profiles, OTP, withdrawal methods
├── 🚘 VehicleManagement      — Vehicles, brands, models, categories
└── 🗺️  ZoneManagement         — Geographic service zones
```

Each module follows this structure:

```
Modules/ModuleName/
├── Entities/          # Eloquent models
├── Http/
│   └── Controllers/   # Module-specific controllers
├── Routes/            # api.php / web.php scoped to module
├── composer.json
└── package.json
```

---

## 💳 Payment Gateways

Cabtale supports **7+ payment gateways** out of the box, configurable per zone from the admin panel.

| Gateway | Region | Package |
|---|---|---|
| ![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white) | Global | `stripe/stripe-php` ^13.9 |
| ![Razorpay](https://img.shields.io/badge/Razorpay-02042B?style=flat-square&logo=razorpay&logoColor=white) | India | `razorpay/razorpay` ^2.9 |
| ![MercadoPago](https://img.shields.io/badge/MercadoPago-009EE3?style=flat-square&logo=mercadopago&logoColor=white) | LATAM | `mercadopago/dx-php` 2.4.3 |
| Iyzico | Turkey | `iyzico/iyzipay-php` ^2.0 |
| Xendit | SEA | `xendit/xendit-php` ^4.1 |
| ![Paystack](https://img.shields.io/badge/Paystack-00C3F7?style=flat-square&logo=paystack&logoColor=white) | Africa | `unicodeveloper/laravel-paystack` ^1.1 |
| CCAvenue | India | Custom integration |
| Cash on Delivery | Universal | Built-in |
| Wallet | Universal | Built-in |

---

## 🚀 Getting Started

### Prerequisites

Ensure the following tools are installed on your system:

| Tool | Minimum Version | Notes |
|---|---|---|
| PHP | 8.1 | With `pdo_mysql`, `mbstring`, `zip`, `gd`, `redis` extensions |
| Composer | 2.x | PHP dependency manager |
| MySQL | 8.x | Primary database |
| Redis | 7.x | Caching, queues, broadcasting |
| Node.js | 18.x | For asset compilation |
| NPM | 9.x | Asset compilation |
| Flutter SDK | 3.3.0+ | For mobile apps |
| Dart SDK | 3.x | Bundled with Flutter |
| Android Studio / Xcode | Latest | For mobile build tools |

---

### Backend Setup (Laravel)

#### 1. Clone the Repository

```bash
git clone https://github.com/teammarktaleworld-crypto/Cabtale.git
cd Cabtale/public_html
```

#### 2. Install PHP Dependencies

```bash
composer install --optimize-autoloader --no-dev
```

#### 3. Configure Environment

```bash
cp .env.example .env
php artisan key:generate
```

Open `.env` and configure your database, Redis, mail, and third-party service credentials (see [Environment Configuration](#-environment-configuration)).

#### 4. Run Database Migrations & Seeders

```bash
php artisan migrate --seed
```

#### 5. Install Passport OAuth Keys

```bash
php artisan passport:install
```

#### 6. Compile Frontend Assets

```bash
npm install
npm run production
```

#### 7. Set Storage Permissions

```bash
chmod -R 775 storage bootstrap/cache
php artisan storage:link
```

#### 8. Start the Development Server

```bash
php artisan serve
```

API will be available at `http://localhost:8000/api`.

#### 9. Start the WebSocket Server (Reverb)

```bash
php artisan reverb:start
```

#### 10. Start the Queue Worker

```bash
php artisan queue:work --daemon
```

> **Production tip:** Use [Supervisor](http://supervisord.org/) to manage queue workers and the Reverb WebSocket server as background daemons.

---

### Flutter Apps Setup

Both mobile apps live under `Cabtale_user/` (passenger app) and `Cabtale_driver/` (driver app).

#### 1. Set Up Firebase

1. Create a Firebase project at [Firebase Console](https://console.firebase.google.com/).
2. Download `google-services.json` (Android) and `GoogleService-Info.plist` (iOS).
3. Place `google-services.json` → `Cabtale_user/android/app/` and `Cabtale_driver/android/app/`.
4. Place `GoogleService-Info.plist` → `Cabtale_user/ios/Runner/` and `Cabtale_driver/ios/Runner/`.

#### 2. Configure API Base URL

Open the configuration file in each app and set your backend URL:

```dart
// Cabtale_user/lib/util/app_constants.dart (or similar)
static const String baseUrl = 'https://your-domain.com/api';
```

#### 3. Install Flutter Dependencies

```bash
# User app
cd Cabtale_user
flutter pub get

# Driver app
cd ../Cabtale_driver
flutter pub get
```

#### 4. Run the Apps

```bash
# Run on connected device / emulator
flutter run
```

#### 5. Build for Production

```bash
# Android APK
flutter build apk --release

# Android App Bundle (Play Store)
flutter build appbundle --release

# iOS (requires macOS + Xcode)
flutter build ios --release
```

---

## ⚙️ Environment Configuration

Below are the key environment variables for the Laravel backend (`.env`):

```dotenv
# ── Application ────────────────────────────────────────────
APP_NAME=Cabtale
APP_ENV=production
APP_MODE=live
APP_DEBUG=false
APP_URL=https://your-domain.com

# ── Database ────────────────────────────────────────────────
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=cabtale_db
DB_USERNAME=cabtale_user
DB_PASSWORD=your_secure_password

# ── Redis ───────────────────────────────────────────────────
REDIS_HOST=127.0.0.1
REDIS_PORT=6379
REDIS_PASSWORD=null

# ── Queues & Broadcasting ───────────────────────────────────
BROADCAST_DRIVER=reverb
CACHE_DRIVER=redis
QUEUE_CONNECTION=redis
SESSION_DRIVER=redis
SESSION_LIFETIME=120

# ── WebSocket (Laravel Reverb) ──────────────────────────────
REVERB_APP_ID=cabtale
REVERB_APP_KEY=your_reverb_key
REVERB_APP_SECRET=your_reverb_secret
REVERB_HOST=0.0.0.0
REVERB_PORT=6015
REVERB_SCHEME=https
REVERB_SSL_CERT_PATH="/etc/ssl/certs/your_cert.crt"
REVERB_SSL_KEY_PATH="/etc/ssl/private/your_key.key"

# ── Pusher (optional, alternative to Reverb) ───────────────
PUSHER_APP_ID=your_pusher_app_id
PUSHER_APP_KEY=your_pusher_key
PUSHER_APP_SECRET=your_pusher_secret
PUSHER_APP_CLUSTER=mt1

# ── Mail ────────────────────────────────────────────────────
MAIL_MAILER=smtp
MAIL_HOST=smtp.your-provider.com
MAIL_PORT=587
MAIL_USERNAME=noreply@your-domain.com
MAIL_PASSWORD=your_mail_password
MAIL_ENCRYPTION=tls
MAIL_FROM_ADDRESS=noreply@your-domain.com
MAIL_FROM_NAME="Cabtale"

# ── Google Maps ─────────────────────────────────────────────
GOOGLE_MAP_API=your_google_maps_api_key

# ── Stripe ──────────────────────────────────────────────────
STRIPE_KEY=pk_live_...
STRIPE_SECRET=sk_live_...

# ── Twilio (SMS) ────────────────────────────────────────────
TWILIO_SID=your_twilio_sid
TWILIO_AUTH_TOKEN=your_twilio_token
TWILIO_FROM=+1234567890

# ── Firebase (Server Key) ───────────────────────────────────
FIREBASE_SERVER_KEY=your_firebase_server_key
```

---

## 🔌 API Overview

All API routes are prefixed with `/api`. Authentication uses **Laravel Sanctum** bearer tokens.

### Authentication

| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/api/customer/auth/registration` | Register new customer |
| `POST` | `/api/customer/auth/login` | Customer email/password login |
| `POST` | `/api/customer/auth/otp-login` | OTP-based login |
| `POST` | `/api/customer/auth/social-login` | Social login (Google/Apple) |
| `POST` | `/api/customer/auth/forget-password` | Initiate password reset |
| `POST` | `/api/customer/auth/reset-password` | Complete password reset |
| `POST` | `/api/driver/auth/registration` | Register new driver |
| `POST` | `/api/driver/auth/login` | Driver login |

### Configuration

| Method | Endpoint | Description |
|---|---|---|
| `GET` | `/api/configurations` | Global app configuration |
| `GET` | `/api/customer/configuration` | Customer-specific configuration |
| `GET` | `/api/config/get-zone-id` | Get zone for current coordinates |
| `GET` | `/api/config/place-api-autocomplete` | Google Places autocomplete |
| `GET` | `/api/config/distance-api` | Distance & duration calculation |
| `GET` | `/api/config/get-payment-methods` | Available payment methods |

### Trips

| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/api/trip/create` | Create a trip request |
| `GET` | `/api/trip/{id}` | Get trip details |
| `PUT` | `/api/trip/{id}/status` | Update trip status |
| `GET` | `/api/trip/history` | Trip history for user/driver |

### Payments

| Method | Endpoint | Description |
|---|---|---|
| `GET` | `/payment-success` | Payment success callback |
| `GET` | `/payment-fail` | Payment failure callback |
| `GET` | `/payment-cancel` | Payment cancellation callback |

> 📚 Full API documentation is available through the admin panel at `/docs` once deployed.

---

## ⚡ Real-time Services

Cabtale uses **Laravel Reverb** (or Pusher as fallback) for all real-time features:

| Feature | Channel Type | Description |
|---|---|---|
| Driver Location Updates | Presence | Live GPS position broadcast to passenger |
| Trip Status Changes | Private | Booking confirmation, pickup, en-route, drop-off |
| In-App Chat | Private | Bi-directional driver ↔ passenger messaging |
| New Trip Requests (Driver) | Private | Instant ride request notifications |
| Push Notifications | FCM | Background/foreground alerts via Firebase |

### Starting Reverb (Production)

```bash
# Start WebSocket server
php artisan reverb:start --host=0.0.0.0 --port=6015

# Or with SSL termination (recommended for production)
php artisan reverb:start --host=0.0.0.0 --port=6015 --tls
```

Add the following to your Supervisor configuration to keep Reverb alive:

```ini
[program:cabtale-reverb]
command=php /var/www/cabtale/public_html/artisan reverb:start --host=0.0.0.0 --port=6015
autostart=true
autorestart=true
user=www-data
redirect_stderr=true
stdout_logfile=/var/log/cabtale-reverb.log
```

---

## 🔐 Security

Cabtale follows industry-standard security practices:

- **OAuth 2.0** — All API access is secured via Laravel Passport tokens
- **API Token Authentication** — Short-lived sanctum tokens for mobile clients
- **HTTPS Enforcement** — All production traffic must be served over TLS/SSL
- **OTP Verification** — Phone number verification via Twilio SMS
- **Password Hashing** — bcrypt with configurable cost factor
- **Rate Limiting** — API throttling on auth endpoints to prevent brute-force
- **Input Validation** — All inputs validated via Laravel Form Requests
- **CORS Configuration** — Strict origin control via `config/cors.php`
- **SQL Injection Prevention** — Eloquent ORM with parameterized queries
- **XSS Protection** — Output escaping in all Blade templates
- **Data Encryption** — Sensitive config values encrypted at rest

---

## 🌐 Deployment

### Recommended Stack

| Component | Recommendation |
|---|---|
| Web Server | Nginx 1.24+ |
| PHP Runtime | PHP-FPM 8.1+ |
| Process Manager | Supervisor |
| SSL | Let's Encrypt / Certbot |
| Cloud | GCP (Compute Engine / Cloud Run) |
| Database | GCP Cloud SQL (MySQL 8) |
| Redis | GCP Memorystore |
| Storage | GCP Cloud Storage |

### Quick Deployment Checklist

```bash
# 1. Pull latest code
git pull origin main

# 2. Install/update dependencies
composer install --optimize-autoloader --no-dev

# 3. Run migrations
php artisan migrate --force

# 4. Clear and warm up caches
php artisan config:cache
php artisan route:cache
php artisan view:cache
php artisan event:cache

# 5. Restart queue workers
php artisan queue:restart

# 6. Restart Reverb (via Supervisor)
supervisorctl restart cabtale-reverb

# 7. Set correct permissions
chown -R www-data:www-data storage bootstrap/cache
chmod -R 775 storage bootstrap/cache
```

### Nginx Configuration Sample

```nginx
server {
    listen 443 ssl http2;
    server_name your-domain.com;

    root /var/www/cabtale/public_html/public;
    index index.php;

    ssl_certificate     /etc/ssl/certs/cabtale.crt;
    ssl_certificate_key /etc/ssl/private/cabtale.key;

    location / {
        try_files $uri $uri/ /index.php?$query_string;
    }

    location ~ \.php$ {
        fastcgi_pass unix:/run/php/php8.1-fpm.sock;
        fastcgi_index index.php;
        include fastcgi_params;
        fastcgi_param SCRIPT_FILENAME $document_root$fastcgi_script_name;
    }

    # WebSocket proxy (Reverb)
    location /app/ {
        proxy_pass http://127.0.0.1:6015;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection "Upgrade";
        proxy_set_header Host $host;
    }
}
```

---

## 📁 Project Structure

```
Cabtale/
├── public_html/               # 🖥  Laravel Backend API
│   ├── Modules/               # 14 domain modules
│   │   ├── AdminModule/
│   │   ├── AuthManagement/
│   │   ├── BusinessManagement/
│   │   ├── ChattingManagement/
│   │   ├── FareManagement/
│   │   ├── Gateways/
│   │   ├── ParcelManagement/
│   │   ├── PromotionManagement/
│   │   ├── ReviewModule/
│   │   ├── TransactionManagement/
│   │   ├── TripManagement/
│   │   ├── UserManagement/
│   │   ├── VehicleManagement/
│   │   └── ZoneManagement/
│   ├── app/                   # Core Laravel application
│   │   ├── Http/              # Controllers, Middleware
│   │   ├── Models/            # Eloquent models
│   │   ├── Events/            # Application events
│   │   ├── Jobs/              # Queue jobs
│   │   ├── Listeners/         # Event listeners
│   │   └── Service/           # Business logic services
│   ├── config/                # Configuration files
│   ├── database/              # Migrations, seeders, factories
│   ├── routes/                # API & web routes
│   ├── resources/             # Views, lang, assets
│   ├── public/                # Web root (compiled assets)
│   ├── storage/               # Logs, uploads, caches
│   └── tests/                 # PHPUnit test suite
│
├── Cabtale_user/              # 📱 Passenger Flutter App
│   ├── lib/
│   │   ├── common_widgets/    # Shared UI components
│   │   ├── data/              # Data layer (models, services)
│   │   ├── features/          # Feature modules
│   │   ├── localization/      # i18n translations
│   │   ├── theme/             # App theming
│   │   └── main.dart          # App entry point
│   ├── android/
│   ├── ios/
│   └── pubspec.yaml
│
└── Cabtale_driver/            # 🚗 Driver Flutter App
    ├── lib/
    │   ├── common_widgets/
    │   ├── data/
    │   ├── features/
    │   ├── localization/
    │   ├── theme/
    │   └── main.dart
    ├── android/
    ├── ios/
    └── pubspec.yaml
```

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/your-feature-name`
3. **Commit** your changes with clear messages: `git commit -m "feat: add driver bidding improvements"`
4. **Push** to your fork: `git push origin feature/your-feature-name`
5. **Open** a Pull Request against `main`

### Coding Standards

- **PHP / Laravel** — Follow [PSR-12](https://www.php-fig.org/psr/psr-12/). Run `./vendor/bin/pint` before committing.
- **Dart / Flutter** — Follow [Effective Dart](https://dart.dev/guides/language/effective-dart). Run `flutter analyze` before committing.

---

## 📄 Copyright

```
© 2026 Team MarktaleWorld Pvt Ltd. All rights reserved.

This software is proprietary and confidential. Unauthorized copying,
modification, distribution, or use of this software, via any medium,
is strictly prohibited without the express written permission of
Team MarktaleWorld Pvt Ltd.
```

---

<p align="center">
  Built with ❤️ by <strong>Team MarktaleWorld Pvt Ltd</strong>
  <br/>
  <img src="https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white"/>
  <img src="https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white"/>
  <img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white"/>
  <img src="https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black"/>
  <img src="https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white"/>
  <img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white"/>
</p>

