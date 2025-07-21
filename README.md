# Laravel Lavissa (Docker + Laravel 10)

Bu proje Laravel 10 tabanlıdır ve Docker ile kolayca ayağa kaldırılabilir. Apple M3/M2/M1 cihazlarla tam uyumludur.

## 🚀 Kurulum (Yeni bir bilgisayarda)

Aşağıdaki adımları sırayla terminalde uygulayarak Laravel Lavissa projesini çalıştırabilirsin:

---

### 1. Repoyu Klonla

```bash
git clone https://github.com/ceobusb/laravel-lavissa.git
cd laravel-lavissa
cp src/.env.example src/.env
docker-compose up -d --build
docker exec -it laravel10-app php artisan key:generate
docker exec -it laravel10-app php artisan migrate
Laravel Uygulaması: http://localhost:8010

PhpMyAdmin: http://localhost:8081

Kullanıcı Adı: laravel

Şifre: secret
