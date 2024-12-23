<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Event-Management

Event-Management is a REST API built with Laravel that allows users to manage events and attendees. It provides a robust platform for creating, updating, viewing, and deleting events, as well as managing event attendees.

### Features

- **User Authentication and Authorization**: Secure user authentication and authorization using Laravel Sanctum.
- **Event Management**: Create, update, view, and delete events.
- **Attendee Management**: Add and remove attendees for events.
- **Rate Limiting**: Protect the API from abuse by limiting the number of requests.
- **Real-time Notifications**: Notify users about event updates and attendee actions.
- **Search and Filter**: Search and filter events based on various criteria.

### API Endpoints

- **Authentication**
  - `POST /login`: Login a user.
  - `POST /logout`: Logout a user.
- **Events**
  - `GET /events`: List all events.
  - `GET /events/{id}`: View a specific event.
  - `POST /events`: Create a new event.
  - `PUT /events/{id}`: Update an existing event.
  - `DELETE /events/{id}`: Delete an event.
- **Attendees**
  - `GET /events/{event_id}/attendees`: List all attendees for an event.
  - `POST /events/{event_id}/attendees`: Add an attendee to an event.
  - `DELETE /events/{event_id}/attendees/{attendee_id}`: Remove an attendee from an event.

### Tools Used

- **Postman**: Used for testing and documenting the API endpoints.

## Getting Started

### Prerequisites

- PHP >= 8.0
- Composer
- Laravel
- MySQL or any other supported database

### Installation

To get started with Job-board, follow these steps:

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/job-board.git
    cd job-board
    ```

2. Install dependencies:
    ```sh
    composer install
    npm install
    npm run dev
    ```

3. Set up the environment:
    ```sh
    cp .env.example .env
    php artisan key:generate
    ```

4. Configure the database in the [.env](http://_vscodecontentref_/0) file and run migrations:
    ```sh
    php artisan migrate
    ```

5. Seed the database with initial data (optional):
    ```sh
    php artisan db:seed
    ```

6. Start the development server:
    ```sh
    php artisan serve
    ```

## Usage

- Visit `http://localhost:8000` in your browser to access the application.
- Register a new account or log in with existing credentials.
- Employers can create and manage job listings.
- Job seekers can search for jobs and apply for them.

## License

Job-board is open-source software licensed under the [MIT license](https://opensource.org/licenses/MIT).

## Page Look
