# 🔄 Git Commands for Remote Deployment

Run these commands in your terminal from the project root directory:

## 📁 Navigate to Project Directory
```bash
cd "/Users/anbschool0010/Desktop/Codeclarity - Update 3"
```

## 🔧 Initialize Git (if not already done)
```bash
git init
```

## 📝 Add All Files
```bash
git add .
```

## 💾 Commit Changes
```bash
git commit -m "Prepare CodeClarity for Render deployment

- Add render.yaml configuration
- Create .env.example template
- Add comprehensive deployment guide
- Update package.json with engines
- Add health check endpoint
- Update .gitignore for production
- Add Dockerfile for containerization"
```

## 🌐 Add Remote Repository
Replace `YOUR_GITHUB_USERNAME` and `YOUR_REPO_NAME` with your actual values:

```bash
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPO_NAME.git
```

## 🚀 Push to Remote
```bash
git branch -M main
git push -u origin main
```

## ✅ Verify Upload
Check your GitHub repository to ensure all files are uploaded correctly.

---

## 🔗 Next: Deploy to Render

After pushing to GitHub:

1. Go to [Render Dashboard](https://dashboard.render.com)
2. Click "New" → "Blueprint" 
3. Connect your GitHub repository
4. Render will detect `render.yaml` automatically
5. Set your environment variables:
   - `OPENAI_API_KEY`
   - `JWT_SECRET` 
   - `GEMINI_API_KEY` (optional)
6. Deploy! 🎉

Your app will be live at: `https://your-app-name.onrender.com`
