# Chirper: A Simple Laravel Blog Project

Chirper is a lightweight social media application built with the Laravel framework, inspired by platforms like Twitter. It allows users to post short messages, or "chirps," and interact with a feed of the latest posts from the community.

## Features

-   **User Authentication:** Secure registration and login system for users.
-   **Create Chirps:** Authenticated users can post new messages to the feed.
-   **Edit and Delete:** Users have full control to edit or delete their own chirps.
-   **Real-time Feed:** The homepage displays the latest 50 chirps from all users.
-   **Eloquent Relationships:** A clear `User` and `Chirp` model relationship.
-   **Blade Components:** A clean and reusable UI built with Laravel Blade components.
-   **Form Validation:** Robust server-side validation to ensure data integrity.

---

## Technical Stack

-   **Backend:** PHP 8.2+ / Laravel 12
-   **Frontend:** Tailwind CSS, DaisyUI, Vite
-   **Database:** SQLite by default, easily configurable for MySQL or PostgreSQL.

---

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

-   PHP >= 8.2
-   Composer
-   Node.js & NPM
-   A database server (SQLite, MySQL, or PostgreSQL)

### Installation

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/abdelaleemadel/chirper.git](https://github.com/abdelaleemadel/chirper.git)
    cd chirper
    ```

2.  **Install PHP dependencies:**

    ```bash
    composer install
    ```

3.  **Install NPM dependencies:**

    ```bash
    npm install
    ```

4.  **Set up your environment file:**
    Copy the `.env.example` file to a new file named `.env`.

    ```bash
    cp .env.example .env
    ```

    Generate a new application key.

    ```bash
    php artisan key:generate
    ```

5.  **Configure your database:**
    Update your `.env` file with your database credentials. For SQLite, you can simply create an empty file:

    ```bash
    touch database/database.sqlite
    ```

6.  **Run the database migrations:**
    This will create the `users` and `chirps` tables in your database.

    ```bash
    php artisan migrate
    ```

7.  **Run the database seeder (Optional):**
    This will populate your database with some sample users and chirps.
    ```bash
    php artisan db:seed
    ```

---

## Usage

1.  **Start the development server:**
    This command will start the Vite server for frontend assets and the PHP development server.

    ```bash
    npm run dev
    ```

2.  **Access the application:**
    Open your browser and navigate to `http://localhost:8000`.

3.  **Register a new user** or log in with the test user created by the seeder:
    -   **Email:** `test@example.com`
    -   **Password:** `password`

You can now start posting, editing, and deleting your own chirps!
