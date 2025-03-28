# StuddyBuddy

![StuddyBuddy Logo](static/images/logo.svg) <!-- Update with your logo path if available -->

**StuddyBuddy** is a web application designed to help students connect, collaborate, and study together. Whether you're creating study rooms, joining peers for focused learning, or managing your study topics, StuddyBuddy provides a seamless platform to enhance your educational experience.

---

## Table of Contents
- [Features](#features)
- [Technologies](#technologies)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## Features
- **User Authentication**: Register, log in, and log out securely.
- **Study Rooms**: Create, update, and join study rooms with topics and descriptions.
- **Topic Management**: Suggest and select topics for study sessions.
- **Search Functionality**: Easily find rooms with a built-in search feature.
- **Responsive Design**: Works across desktop and mobile devices.
- **User Profiles**: Personalized greetings and profile display with capitalized usernames.

---

## Technologies
- **Backend**: Django (Python)
- **Frontend**: HTML, CSS, JavaScript
- **Database**: SQLite (default; configurable for PostgreSQL, MySQL, etc.)
- **Static Files**: Django’s static file handling for images and assets
- **Dependencies**: Managed via `requirements.txt`

---

## Installation

### Prerequisites
- Python 3.8+ (recommended: 3.12 as per your setup)
- Git
- Virtualenv (optional but recommended)

### Steps
1. **Clone the Repository**
   ```bash
   git clone https://github.com/Ibrahimkazi18/StuddyBuddy.git
   cd StuddyBuddy
   ```

2. **Set Up a Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure the Database**
   - Ensure your `settings.py` has the correct database settings (default is SQLite).
   - Run migrations:
     ```bash
     python manage.py makemigrations
     python manage.py migrate
     ```

5. **Create a Superuser (Optional)**
   - To access the Django admin panel:
     ```bash
     python manage.py createsuperuser
     ```

6. **Collect Static Files**
   - For development, ensure static files are served:
     ```bash
     python manage.py collectstatic
     ```

7. **Run the Development Server**
   ```bash
   python manage.py runserver
   ```
   - Open your browser and visit `http://localhost:8000`.

---

## Usage
1. **Register an Account**: Go to `/register/` to create a new user.
2. **Log In**: Use `/login/` to access your account.
3. **Create a Study Room**: Navigate to `/create-room/` and fill out the form.
4. **Update a Room**: Visit `/room/<id>/update/` to modify an existing room (requires authentication).
5. **Search Rooms**: Use the search bar on the homepage to find study rooms by keyword.
6. **Log Out**: Click "Logout" from the header when done.

---

## Project Structure
```
StuddyBuddy/
├── base/               # Main app directory
│   ├── migrations/     # Database migrations
│   ├── static/         # Static files (CSS, JS, images)
│   ├── templates/      # HTML templates
│   ├── views.py        # View logic
│   ├── models.py       # Database models (e.g., Room, Topic)
│   └── forms.py        # Form definitions (e.g., RoomForm)
├── studdybuddy/        # Project settings
│   ├── settings.py     # Configuration
│   └── urls.py         # Project-wide URL routing
├── manage.py           # Django management script
└── requirements.txt    # Python dependencies
```

---

## Contributing
We welcome contributions to make StuddyBuddy even better! Here’s how you can help:

1. **Fork the Repository**
   - Click the "Fork" button at the top of this page.

2. **Clone Your Fork**
   ```bash
   git clone https://github.com/<your-username>/StuddyBuddy.git
   ```

3. **Create a Branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

4. **Make Changes**
   - Write clean, documented code.
   - Test your changes locally.

5. **Commit and Push**
   ```bash
   git add .
   git commit -m "Add your descriptive message here"
   git push origin feature/your-feature-name
   ```

6. **Submit a Pull Request**
   - Go to the original repository and create a pull request from your branch.

### Guidelines
- Follow PEP 8 for Python code.
- Write meaningful commit messages.
- Update documentation (e.g., this README) if needed.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contact
- **Author**: Ibrahim Kazi
- **GitHub**: [Ibrahimkazi18](https://github.com/Ibrahimkazi18)
- **Email**: [ibirfkazi@gmail.com](mailto:ibirfkazi@gmail.com) 

Feel free to open an issue on GitHub if you encounter bugs or have feature requests!

---