# Employee Management System
This Application is using Laravel, Materialize-css version 1.0.0 alpha-4 , material icons.

steps to create laravel project

1. Run this command in your command-line (you should be inside htdocs)
    - composer create-project --prefer-dist laravel/laravel ProjectNAme

2. Configuring our Laravel application
    - After installing our Laravel application we will need to configure our database for it to work.
    - Go to http://localhost/phpmyadmin/
    - Create a new Database by clicking on new 
    - Name it employees_db and click Create
    - Now that we have a database we can proceed to set up the application to work with the database.

   - Open your file explorer and navigate to project folder
   - Open the .env file in your code editor
   - Change the following in the file:-

    ```
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=employees_db
    DB_USERNAME=root
    DB_PASSWORD=
    
    ```
    
composer --> This is a dependency management software for PHP.

1. install Composer first, then run this command in your command-line (you should be inside your project directory).
    ```
    composer install
    (OR)
    composer install --ignore-platform-reqs
    (OR)
    composer update --ignore-platform-reqs
    ```
2. generate application key.
    ```
    php artisan key:generate
    ```
3. create database tables.
    ```
    php artisan migrate
    ```
4. create a default admin and genders.
    ```
    php artisan db:seed
    ```

5. clear config (only if you make changes to .env file and restart the server if you are using laravel dev server).
    ```
    php artisan config:clear
    ```

6. Link the storage folder for images.
    ```
    php artisan storage:link
    ```
    
7. Start the development server.
    ```
    php artisan serve
    ```
    
> In Laravel, all the requests are directed to index.php in public directory so, please use a Virtual Host instead of opening it from http://localhost/your-laravel-project/public (It doesn't work that way).

# Admin Credentials
   ```
   username: admin
   Email :- admin@gmail.com
   Password :- admin123
   ```
   

 
