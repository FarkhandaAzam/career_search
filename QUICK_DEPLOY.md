# ⚡ Quick Deploy - 5 Minutes

## 🎯 Easiest Way: Render.com

### Step 1: Push to GitHub
```bash
git add .
git commit -m "Ready for deployment"
git push origin main
```

### Step 2: Deploy on Render
1. Go to: https://render.com
2. Sign up with GitHub (FREE)
3. Click **"New +"** → **"Web Service"**
4. Select your repository: `career_search`
5. Settings:
   - **Name**: `career-search`
   - **Build Command**: `pip install -r requirements.txt`
   - **Start Command**: `gunicorn app:app`
6. Click **"Create Web Service"**
7. Wait 5-10 minutes
8. ✅ **DONE!** Your site is live!

### Your Live URL:
`https://career-search.onrender.com`

---

## 🔗 Alternative: Railway (Even Faster)

1. Go to: https://railway.app
2. Sign up with GitHub
3. Click **"New Project"** → **"Deploy from GitHub"**
4. Select `career_search`
5. ✅ **DONE!** Auto-deploys!

---

## ✅ After Deployment

Test these URLs:
- `/` - Home page
- `/login` - Login
- `/quiz` - Career quiz
- `/gpa` - GPA calculator
- `/consultation` - Book appointment
- `/quiz-settings/login` - Admin (admin202@gmail.com / admin202)

---

## 🎉 That's It!

Your complete website is now live! 🚀

