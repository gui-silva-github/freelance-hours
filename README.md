<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

# FreelanceHours

**FreelanceHours** is a dynamic project management platform where users can view available projects and submit proposals based on the number of hours they are willing to dedicate.

The unique aspect of the system is its reverse auction mechanism, where the freelancer who can complete the project in the least amount of time ranks first and is assigned the project.

<hr>

<img src="https://raw.githubusercontent.com/rocketseat-education/freelancehours-curso-php/refs/heads/main/.github/preview.png">

<hr>

## Recursos

This project is built using PHP with the Laravel framework, following the MVC architecture to ensure clean code and structure. It incorporates:

- Controllers, models, and views to handle the business logic and presentation layers.
- SQLite as the database, leveraging migrations for version control and database structure, and factories and seeders to populate the database with test data.
- Form validations to ensure accurate inputs.
- A responsive and interactive user interface, enhanced by Livewire, to provide real-time feedback and dynamic behavior.

<hr>

## Instalação do Projeto

Follow the steps below to install and configure the FreelanceHours project on your local machine:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/gui-silva-github/freelance-hours.git
   cd freelance-hours
   ```

2. **Install PHP dependencies: Run the following command to install the necessary dependencies:**
   ```bash
   composer install
   ```

3. **Install Node.js dependencies: After installing the PHP dependencies, run:**
   ```bash
   npm install
   ```

4. **Create the .env file**
   If the .env file does not exist, create it based on the example file:
   ```bash
   cp .env.example .env
   ```
   Then, edit the .env file to configure the environment variables, especially the database settings.

5. **Generate the application key:**
   Run the following command to generate the application key:
   ```bash
   php artisan key:generate
   ```

6. **Create the SQLite database:**
   Ensure the database.sqlite file exists in the database directory. If it doesn’t, create it:
   ```bash
   touch database/database.sqlite
   ```

7. **Run the migrations:**
   To create the tables in the database, run:
   ```bash
   php artisan migrate
   ```

8. **(Optional) Seed the database with sample data:**
   If you want to seed the database with example data, run:
   ```bash
   php artisan migrate:fresh --seed
   ```

9. **Compile the assets:**
   To compile the front-end assets, run:  
   ```bash
   npm run dev
   ```

10. **Start the server:**
    Finally, start the Laravel built-in server:
    ```bash
    php artisan serve
    ```
The application will be available at http://localhost:8000/.

<hr>

## Licença

Este projeto está licenciado sob a [MIT license](https://opensource.org/licenses/MIT).
