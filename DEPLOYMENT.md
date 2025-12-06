# 🚀 Complete Website Deployment Guide

## Option 1: Render.com (Recommended - FREE)

### Step 1: Prepare Your Repository
1. Make sure all files are committed and pushed to GitHub
2. Files needed:
   - `app.py`
   - `requirements.txt`
   - `Procfile` or `render.yaml`
   - All templates and static files

### Step 2: Deploy on Render
1. Go to [https://render.com](https://render.com)
2. Sign up/Login with GitHub
3. Click **"New +"** → **"Web Service"**
4. Connect your GitHub repository: `FarkhandaAzam/career_search`
5. Configure:
   - **Name**: `career-search` (or any name)
   - **Environment**: `Python 3`
   - **Build Command**: `pip install -r requirements.txt`
   - **Start Command**: `gunicorn app:app`
   - **Plan**: Free
6. Click **"Create Web Service"**
7. Wait for deployment (5-10 minutes)
8. Your site will be live at: `https://career-search.onrender.com` (or your custom name)

### Step 3: Custom Domain (Optional)
1. In Render dashboard, go to Settings
2. Add your custom domain
3. Update DNS records as instructed

---

## Option 2: Railway.app (FREE)

### Step 1: Deploy
1. Go to [https://railway.app](https://railway.app)
2. Sign up with GitHub
3. Click **"New Project"** → **"Deploy from GitHub repo"**
4. Select `career_search` repository
5. Railway will auto-detect Flask
6. Add environment variable: `PORT=5000`
7. Deploy!

Your site will be live at: `https://your-app-name.railway.app`

---

## Option 3: PythonAnywhere (FREE)

### Step 1: Setup
1. Go to [https://www.pythonanywhere.com](https://www.pythonanywhere.com)
2. Create a free account
3. Open a Bash console

### Step 2: Clone and Setup
```bash
cd ~
git clone https://github.com/FarkhandaAzam/career_search.git
cd career_search
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### Step 3: Configure Web App
1. Go to **Web** tab
2. Click **"Add a new web app"**
3. Choose **Flask** → **Python 3.10**
4. Set path: `/home/yourusername/career_search/app.py`
5. Click **"Reload"**

Your site will be live at: `https://yourusername.pythonanywhere.com`

---

## Option 4: Heroku (Paid - $5/month)

### Step 1: Install Heroku CLI
Download from [https://devcenter.heroku.com/articles/heroku-cli](https://devcenter.heroku.com/articles/heroku-cli)

### Step 2: Deploy
```bash
heroku login
heroku create career-search-app
git push heroku main
heroku open
```

---

## 🔧 Important Configuration

### Environment Variables (if needed)
Add these in your hosting platform:
- `FLASK_ENV=production`
- `PORT=5000` (usually auto-set)
- `SECRET_KEY=your-secret-key-here` (for production)

### Database
- SQLite database will be created automatically in `instance/` folder
- For production, consider using PostgreSQL (Render provides free PostgreSQL)

---

## ✅ After Deployment

1. **Test your site**: Visit your live URL
2. **Check admin login**: `/quiz-settings/login`
   - Email: `admin202@gmail.com`
   - Password: `admin202`
3. **Test all features**:
   - Login/Signup
   - Quiz
   - GPA Calculator
   - Consultation booking
   - Profile

---

## 🐛 Troubleshooting

### Build Fails
- Check `requirements.txt` has all dependencies
- Ensure Python version matches (3.8+)

### App Crashes
- Check logs in hosting platform
- Verify `Procfile` or start command is correct
- Ensure port is set correctly

### Database Issues
- Make sure `instance/` folder is writable
- Check database path in `app.py`

---

## 📝 Quick Deploy Checklist

- [ ] All files committed to GitHub
- [ ] `requirements.txt` updated
- [ ] `Procfile` or `render.yaml` created
- [ ] `app.py` configured for production
- [ ] Repository is public (for free tiers)
- [ ] Deployed and tested

---

## 🎉 Success!

Once deployed, your complete Career Search website will be live with:
- ✅ Full Flask application
- ✅ All features working
- ✅ Database functionality
- ✅ Admin panel
- ✅ All routes accessible

**Share your live URL!** 🚀

