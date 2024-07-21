# Study-Bud App

Welcome to the Study-Bud App! This application helps students and learners connect with each other to form study groups, share resources, and support one another in their educational journeys.

## Features
- User authentication (sign up, log in, log out)
- Create and manage study groups
- Join existing study groups
- Chat functionality within study groups
- Share resources (files, links, notes) within groups
- Search for study groups by subject or location

## Installation
### Prerequisites
- Python 3.7+
- PostgreSQL

### Setup
1. Clone the repository:
    ```sh
    git clone https://github.com/whoisrobinjha/Study-Bud-App.git
    cd Study-Bud-App
    ```

2. Create a virtual environment and activate it:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

4. Set up the database:
    - Create a PostgreSQL database named `studybud`.
    - Configure your database settings in the `settings.py` file.

5. Apply the database migrations:
    ```sh
    python manage.py migrate
    ```

6. Start the development server:
    ```sh
    python manage.py runserver
    ```

## Usage
1. Open your browser and navigate to `http://127.0.0.1:8000/` to access the Study-Bud App.
2. Sign up for a new account or log in with your existing credentials.
3. Create a new study group or join an existing one.
4. Start collaborating with your study buddies!

## API Documentation
The Study-Bud App provides a RESTful API for interacting with the backend. Here are some of the main endpoints:

- `POST /api/auth/signup/`: Create a new user account.
- `POST /api/auth/login/`: Log in to an existing account.
- `GET /api/groups/`: Retrieve a list of all study groups.
- `POST /api/groups/`: Create a new study group.
- `GET /api/groups/{id}/`: Retrieve details of a specific study group.
- `POST /api/groups/{id}/join/`: Join a specific study group.
- `POST /api/groups/{id}/chat/`: Send a message in the group's chat.

For detailed API documentation, refer to the `api` folder in the repository.

---

Thank you for using the Study-Bud App! We hope it enhances your learning experience.
