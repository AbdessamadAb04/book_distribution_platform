# Book Distribution Platform (Backend)

Welcome to the **Book Distribution Platform** backend project! This is a robust and secure Django-based API built using **Django REST Framework (DRF)** and **SimpleJWT** for modern authentication.

Currently, the platform provides a solid foundation with user management and a notes system, ready to be expanded into a full-scale book distribution service.

## 🚀 Features

-   **User Authentication**: Secure registration and login using JSON Web Tokens (JWT).
-   **Token Refreshing**: Seamless session management with Access and Refresh tokens.
-   **Notes API**: A complete system for users to create, view, and manage personal notes. (Placeholder for Book management).
-   **CORS Enabled**: Configured with `django-cors-headers` for easy frontend integration.
-   **Secure Configuration**: Uses `python-dotenv` for environment variable management.

## 🛠️ Tech Stack

-   **Framework**: [Django 5.2](https://www.djangoproject.com/)
-   **API Toolkit**: [Django REST Framework](https://www.django-rest-framework.org/)
-   **Authentication**: [SimpleJWT](https://django-rest-framework-simplejwt.readthedocs.io/)
-   **Database**: SQLite (Development)
-   **Environment**: [python-dotenv](https://github.com/theskumar/python-dotenv)

## 🛠️ Getting Started

### Prerequisites

-   Python 3.10+
-   `pip` (Python package manager)

### Installation

1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/AbdessamadAb04/book_distribution_platform.git
    cd book_distribution_platform
    ```

2.  **Create a Virtual Environment**:
    ```bash
    python -m venv env
    # On Windows:
    .\env\Scripts\activate
    # On macOS/Linux:
    source env/bin/activate
    ```

3.  **Install Dependencies**:
    ```bash
    pip install -r backend/backend/requirements.txt
    ```

4.  **Configuration**:
    Create a `.env` file in the `backend/` directory and add your `SECRET_KEY` and other sensitive configurations.

5.  **Run Migrations**:
    ```bash
    cd backend
    python manage.py migrate
    ```

6.  **Run the Development Server**:
    ```bash
    python manage.py runserver
    ```

## 📡 API Endpoints

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/api/user/register/` | Register a new user |
| `POST` | `/api/token/` | Obtain Access & Refresh tokens |
| `POST` | `/api/token/refresh/` | Refresh the Access token |
| `GET/POST` | `/api-auth/` | DRF Browsable API login/logout |

## 📁 Project Structure

```text
backend/
    api/            # App logic: Models, Views, Serializers
    backend/        # Core settings, URLs, and WSGI/ASGI config
    manage.py       # Django project manager
.gitignore          # Git exclusion rules
README.md           # Project documentation
```

## ⚖️ License

This project is open-source and available under the MIT License.
