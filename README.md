# Login SSO Project

This project is a Laravel-based web application that provides a secure and efficient way to manage user authentication across multiple applications or services.

## Installation

### Prerequisites

Before you begin, ensure you have met the following requirements:

-   You have installed PHP version ^8.1.
-   You have installed Composer.
-   You have installed Node.js and npm.

### Installing Dependencies

Install the necessary dependencies:

```
npm install
composer install
```

### Setting Up Environment Variables

Copy the `.env.example` file to `.env`:

```
cp .env.example .env
```

Update the Google credentials at `.env`:

```
GOOGLE_CLIENT_ID=440094953479-vqjg82gsn2s03qbs98v8b5ts67brmv7b.apps.googleusercontent.com
GOOGLE_CLIENT_SECRET=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
GOOGLE_REDIRECT_URL=http://127.0.0.1:8000/auth/google/callback
```

Create new credentials here:
https://console.cloud.google.com/apis/credentials

### Generating Application Key

Generate the application key:

```
php artisan key:generate
```

### Running Migrations

Run the database migrations:

```
php artisan migrate:fresh
```

### Starting the Server

Start the development server:

```
npm run dev
php artisan serve
```
