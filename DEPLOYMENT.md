# Deployment Guide - FRAUD-X

## Free Deployment Options

### Option 1: Streamlit Cloud (Recommended - Easiest)
The Streamlit dashboard is the most complete and user-facing component.

**Steps:**
1. Push your code to GitHub
2. Go to [share.streamlit.io](https://share.streamlit.io)
3. Click "New app"
4. Connect your GitHub repository
5. Select the repository
6. Main file path: `dashboards/app.py`
7. Click "Deploy"

**Your app will be available at:** `https://your-app-name.streamlit.app`

---

### Option 2: Vercel (React Web App)
For the React frontend in the `web/` directory.

**Steps:**
1. Push your code to GitHub
2. Go to [vercel.com](https://vercel.com)
3. Click "New Project"
4. Import your GitHub repository
5. Root directory: `web`
6. Build command: `npm run build`
7. Output directory: `dist`
8. Click "Deploy"

**Your app will be available at:** `https://your-app-name.vercel.app`

---

### Option 3: Render (FastAPI Backend)
For the Python API backend.

**Steps:**
1. Push your code to GitHub
2. Go to [render.com](https://render.com)
3. Click "New +"
4. Select "Web Service"
5. Connect your GitHub repository
6. Build command: `pip install -r requirements.txt`
7. Start command: `uvicorn api.main:app --host 0.0.0.0 --port $PORT`
8. Click "Deploy"

**Your API will be available at:** `https://your-app-name.onrender.com`

---

## Quick Start (Streamlit Cloud)

1. **Create a GitHub repository** if you don't have one:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/your-username/fraud-x.git
   git push -u origin main
   ```

2. **Deploy to Streamlit Cloud:**
   - Visit [share.streamlit.io](https://share.streamlit.io)
   - Click "New app"
   - Select your repository
   - Main file: `dashboards/app.py`
   - Click "Deploy"

3. **Your live link will be ready in 2-3 minutes!**

---

## Files Already Prepared
✅ `requirements.txt` - Python dependencies
✅ `.streamlit/config.toml` - Streamlit configuration
✅ `web/package.json` - React dependencies

---

## Notes
- All deployment options are **100% free**
- Streamlit Cloud is the **easiest and fastest** option
- The dashboard includes all features: live scanner, performance metrics, data insights
