# Laravel-API
## Introduction

This is a Laravel API project that demonstrates how to set up authentication using Laravel Sanctum. The project includes basic API functionalities like user registration, login, and product management.

## Requirements

- PHP 8.2 or higher
- Composer
- MySQL or any other supported database
- Laravel 10 or higher

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/MrxD69/Laravel-API.git
   cd Laravel-API
2. **Install Dependencies**

   Use Composer to install PHP dependencies:
   ```bash
   composer install

3. **Set Up environment Variables**

   copy ".env.example" to ".env"
   ```bash
   cp .env.example .env
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=laravel  
   DB_USERNAME=root     //default
   DB_PASSWORD=
   ```
4. **Generate Application Key**

   generate the laravel application key
   ```bash
   php artisan key:generate
   ```
5. **Run Migrations**
   Migrate the database
   ```bash
   php artisan migrate
   ```
## Usage
### API Endpoints
- Register: `POST /api/register`
- Login: `POST /api/login`
- Product List: `GET /api/products`
- Product Create: `POST /api/products`
- Product Show: `GET /api/products/{id}`
- Product Update: `PUT /api/products/{id}`
- Product Delete: `DELETE /api/products/{id}`

### Testing with Postman
1. Set Headers

In Postman, add the following headers for requests that require authentication:
```json
{
    "Accept": "application/json",
    "Authorization": "Bearer <your-access-token>"
}
```
2. Testing Endpoints

- Register a new user.
- Log in to get the authentication token.
- Use the token to access protected routes like creating, updating, and deleting products.

## Contributing
Feel free to fork this project and submit pull requests.

## License
This project is licensed under the MIT License.





