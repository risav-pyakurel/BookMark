# Bookmark Application

## Overview
The Bookmark Application is a Django-based web application designed to help users save, organize, and manage their favorite web links efficiently. It provides a user-friendly interface for creating, editing, and categorizing bookmarks, making it easier to access important resources quickly.

## Features
- **User Authentication**: Secure user registration, login, and password management.
- **Bookmark Management**: Add, edit, delete, and categorize bookmarks.
- **Search Functionality**: Quickly find bookmarks using keywords.
- **Responsive Design**: Optimized for both desktop and mobile devices.
- **Static File Handling**: Efficient management of CSS, JavaScript, and images.
- **Database Integration**: Uses PostgreSQL for reliable data storage.


## Project Structure
```
bookmark/
├── account/          # User authentication and account management
├── core/             # Core application settings and configurations
├── images/           # Image-related functionalities
├── staticfiles/      # Collected static files for production
├── templates/        # HTML templates for the application
├── manage.py         # Django management script
├── requirements.txt  # Python dependencies
├── Dockerfile        # Docker configuration for containerization
├── docker-compose.yml # Docker Compose configuration
```

## Installation

### Prerequisites
- Python 3.12
- Docker and Docker Compose
- PostgreSQL


### Steps
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd bookmark
   ```
2. Build and run the application using Docker:
   ```bash
   docker-compose up --build
   ```
3. Access the application at `http://localhost:8000`.

## Environment Variables
Create a `.env` file in the root directory with the following variables:
```
POSTGRES_USER=
POSTGRES_PASSWORD=
POSTGRES_DB=bookmark
REDIS_HOST=redis
REDIS_PORT=6379
DJANGO_SECRET_KEY=<your-secret-key>
DEBUG=True
```

## Usage
- Register a new account or log in with existing credentials.
- Add bookmarks by providing a title, URL, and optional description.
- Organize bookmarks into categories for better management.
- Use the search bar to find bookmarks quickly.

## Technologies Used
- **Backend**: Django
- **Frontend**: HTML, CSS, JavaScript
- **Database**: PostgreSQL
- **Containerization**: Docker

## Development
To run the application locally without Docker:
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Apply migrations:
   ```bash
   python manage.py migrate
   ```
3. Run the development server:
   ```bash
   python manage.py runserver
   ```

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes and push them to your fork.
4. Submit a pull request with a detailed description of your changes.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contact
For any inquiries or feedback, please contact [pyakurel.risav@gmail.com].
