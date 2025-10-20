# shop-management-system
In this milestone, I set up the Laravel backend project, configure authentication using Laravel Sanctum for SPA, implement user and branch management with RBAC basics, and create the initial database schema with migrations. The frontend is initialized with Vue 3 (Composition API), Vite, Pinia, vue-router, Bootstrap 5, and SweetAlert2.

Prerequisites

Docker & Docker Compose Node.js 18+ Composer 2+

Local Development

Clone the repo: git clone Copy .env.example to .env in /backend and configure DB (e.g., DB_HOST=db, DB_DATABASE=shop_db, DB_USERNAME=root, DB_PASSWORD=root). Run docker-compose up -d to start services (nginx, php-fpm, mariadb). In backend container: composer install, php artisan key:generate, php artisan migrate --seed In frontend: npm install, npm run dev Access frontend at http://localhost:5173, API at http://localhost/api Demo credentials: Owner - email: owner@example.com, password: password

Environment variables in .env:

APP_URL=http://localhost FRONTEND_URL=http://localhost:5173 (for CORS)

Run tests: php artisan test (basic auth tests included).
