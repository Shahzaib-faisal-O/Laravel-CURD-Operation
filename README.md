# Laravel 8 CRUD Application

This is a simple Laravel 8 CRUD (Create, Read, Update, Delete) application for managing products. The application demonstrates how to create a resource controller, define routes, and use Blade templates for the frontend.

---

## Installation Instructions

### Step 1: Clone the Repository

```bash
git clone https://github.com/Shahzaib-faisal-O/Laravel-CURD-Operation.git
cd CurdOpeartion
```

### Step 2: Install Laravel

Run the following command to install Laravel dependencies:

```bash
composer install
```

### Step 3: Set Up Environment Configuration

Copy the `.env.example` file and rename it to `.env`:

```bash
cp .env.example .env
```

Update the following database credentials in the `.env` file:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_database_username
DB_PASSWORD=your_database_password
```

### Step 4: Generate Application Key

Run the following command to generate an application key:

```bash
php artisan key:generate
```

### Step 5: Run Migrations

Run the database migrations to create the necessary tables:

```bash
php artisan migrate
```

### Step 6: Serve the Application

Start the development server:

```bash
php artisan serve
```

Open your browser and navigate to:

```
http://localhost:8000/products
```

---

## Features

1. **Product Management**

    - Add a new product
    - View product details
    - Edit product details
    - Delete a product

2. **Pagination**: Products are paginated for better user experience.

3. **Validation**: Form inputs are validated before submission.

---

## Project Structure

### Routes

`routes/web.php`
Defines the resource routes for the Product CRUD operations.

### Controller

`app/Http/Controllers/ProductController.php`
Handles the business logic for managing products.

### Model

`app/Models/Product.php`
Defines the `Product` model and its fillable attributes.

### Views

`resources/views/products/`
Contains Blade templates for displaying the product list, forms, and details.

---

## File Structure

```
├── app
│   ├── Http
│   │   └── Controllers
│   │       └── ProductController.php
│   ├── Models
│       └── Product.php
├── database
│   └── migrations
│       └── create_products_table.php
├── resources
│   └── views
│       └── products
│           ├── layout.blade.php
│           ├── index.blade.php
│           ├── create.blade.php
│           ├── edit.blade.php
│           └── show.blade.php
└── routes
    └── web.php
```

---

## Dependencies

-   Laravel 8.x
-   PHP 7.4+
-   MySQL

---

## Commands Summary

-   **Install dependencies**: `composer install`
-   **Run migrations**: `php artisan migrate`
-   **Serve application**: `php artisan serve`

---

## Screenshots

1. **Product Listing**:
   Displays a paginated list of products with options to view, edit, or delete.

2. **Add Product**:
   Form to add a new product.

3. **Edit Product**:
   Form to update an existing product's details.

4. **Show Product**:
   View detailed information about a product.

---

# Output

![Produts Page](screenshot\ProdutsView.PNG)

## License

This project is open-source and available under the [MIT License](LICENSE).
