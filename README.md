# Career Search

A comprehensive career guidance platform that helps students discover their ideal career path through personality assessments, GPA tracking, and professional consultations.

## 🌟 Features

- **Personality-based Career Quiz**: Take a comprehensive quiz to discover your career personality traits
- **GPA Calculator**: Track and calculate your GPA across multiple subjects
- **Professional Counseling**: Book appointments with experienced career counselors
- **Personalized Recommendations**: Get career recommendations based on your personality and academic performance
- **User Profile Management**: Manage your personal information and track your progress
- **Admin Panel**: Admin interface for managing quiz questions and consultants

## 🚀 Live Demo

**GitHub Pages**: [https://farkhandaazam.github.io/career_search/](https://farkhandaazam.github.io/career_search/)

> **Note**: The GitHub Pages site shows a landing page. For the full Flask application, see deployment options below.

## 📋 Prerequisites

- Python 3.8 or higher
- pip (Python package manager)

## 🛠️ Installation

1. Clone the repository:
```bash
git clone https://github.com/FarkhandaAzam/career_search.git
cd career_search
```

2. Create a virtual environment:
```bash
python -m venv venv
```

3. Activate the virtual environment:
   - **Windows**:
     ```bash
     venv\Scripts\activate
     ```
   - **Linux/Mac**:
     ```bash
     source venv/bin/activate
     ```

4. Install dependencies:
```bash
pip install -r requirements.txt
```

## ▶️ Running the Application

### Windows:
```bash
run.bat
```

### Linux/Mac:
```bash
python app.py
```

The application will be available at `http://127.0.0.1:5000`

## 📦 Deployment

### Option 1: Render (Recommended)
1. Push your code to GitHub
2. Go to [Render](https://render.com)
3. Create a new Web Service
4. Connect your GitHub repository
5. Set build command: `pip install -r requirements.txt`
6. Set start command: `python app.py`
7. Deploy!

### Option 2: Heroku
1. Install Heroku CLI
2. Login: `heroku login`
3. Create app: `heroku create your-app-name`
4. Deploy: `git push heroku main`

### Option 3: Railway
1. Go to [Railway](https://railway.app)
2. Connect your GitHub repository
3. Railway will auto-detect Flask and deploy

## 🔐 Admin Access

- **Email**: admin202@gmail.com
- **Password**: admin202

Access the admin panel at `/quiz-settings/login`

## 📁 Project Structure

```
career_search/
├── app.py                 # Main Flask application
├── models.py              # Database models
├── forms.py               # Form definitions
├── requirements.txt       # Python dependencies
├── index.html            # GitHub Pages landing page
├── static/               # Static files (CSS, JS, images)
│   ├── css/
│   ├── js/
│   └── images/
├── templates/            # HTML templates
│   ├── splash.html
│   ├── login.html
│   ├── home.html
│   └── ...
└── instance/            # Database files
    └── career_search.db
```

## 🛣️ Routes

- `/` - Splash/Welcome page
- `/login` - User login
- `/signup` - User registration
- `/home` - Dashboard
- `/quiz` - Career personality quiz
- `/gpa` - GPA calculator
- `/consultation` - Counselor booking
- `/profile` - User profile
- `/quiz-settings` - Admin panel

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Farkhanda Azam**
- GitHub: [@FarkhandaAzam](https://github.com/FarkhandaAzam)

## 🙏 Acknowledgments

- Flask framework
- All contributors and users

---

⭐ If you find this project helpful, please give it a star!
