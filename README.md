# Laravel Starter Kit with Filament, Breeze, and Spatie Login Link

This is a starter kit for Laravel projects that includes:

- **Filament**: A modern and powerful admin panel for Laravel.
- **Breeze**: A simple and minimal authentication kit for Laravel.
- **Spatie Login Link**: A package that provides passwordless login via a unique login link displayed on the screen.

## What's Included?

- **Laravel**: PHP framework for web development.
- **Filament**: Elegant and customizable admin panel.
- **Breeze**: Authentication scaffolding with support for Blade, Vue, or React.
- **Spatie Laravel Login Link**: Passwordless login using unique login links.

## Requirements

- PHP >= 8.2
- Composer
- Node.js (for asset compilation)
- Database (MySQL, PostgreSQL, SQLite, etc.)

## Local Development Setup

Follow these steps to set up the project locally:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/patriciomartinns/laravel-filament-breeze example
   cd example
   
   ## Or
   laravel new example --using=patriciomartinns/laravel-filament-breeze
   ```

2. **Install PHP dependencies**:
   ```bash
   composer install
   ```

3. **Install Node.js dependencies**:
   ```bash
   npm install
   ```

4. **Set up the environment**:
    - Copy the `.env.example` file to `.env`:
      ```bash
      cp .env.example .env
      ```
    - Configure the environment variables in the `.env` file, such as `DB_DATABASE`, `DB_USERNAME`, and `DB_PASSWORD`.

5. **Generate the application key**:
   ```bash
   php artisan key:generate
   ```

6. **Run migrations**:
   ```bash
   php artisan migrate
   ```

7. **Seed the database**:
    - Run the seeder to populate the default user (defined in `DatabaseSeeder`):
      ```bash
      php artisan db:seed
      ```

8. **Compile assets**:
   ```bash
   npm run dev
   ```

9. **Start the development server**:
   ```bash
   composer run dev
   ```

10. **Access the project**:
    - Open your browser and go to `http://localhost:8000`.

This will generate a unique login link for the specified email address.

## Contributing

If you'd like to contribute to this project, follow these steps:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/new-feature`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature/new-feature`).
5. Open a Pull Request.