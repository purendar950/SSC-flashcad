# How to Upload to GitHub

## 🎯 Why Upload to GitHub?

When you upload to GitHub, your website will be accessible online at:
```
https://YOUR-USERNAME.github.io/REPO-NAME/Index-Clean.html
```

No need for a local server anymore - anyone can access it from anywhere!

## 📋 Step-by-Step Guide

### Step 1: Create a GitHub Account (if you don't have one)
1. Go to https://github.com
2. Click "Sign up"
3. Follow the instructions

### Step 2: Create a New Repository

1. Click the **"+"** icon in top-right corner
2. Select **"New repository"**
3. Fill in:
   - **Repository name**: `ssc-vocabulary` (or any name you like)
   - **Description**: "SSC Exam Vocabulary Flashcard App"
   - **Public** ✅ (so it can be hosted)
   - **Add a README file** ✅
4. Click **"Create repository"**

### Step 3: Upload Your Files

#### Option A: Using GitHub Web Interface (Easiest)

1. In your new repository, click **"Add file"** → **"Upload files"**
2. Drag and drop these files:
   - `Index-Clean.html`
   - `vocab.html`
   - `README.md`
   - `QUICK_START.md`
3. Scroll down and click **"Commit changes"**

#### Option B: Using Git Command Line

```bash
# Navigate to your folder
cd path/to/your/folder

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: SSC Vocabulary App"

# Connect to GitHub (replace YOUR-USERNAME and REPO-NAME)
git remote add origin https://github.com/YOUR-USERNAME/REPO-NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 4: Enable GitHub Pages

1. In your repository, click **"Settings"** (top menu)
2. Scroll down to **"Pages"** (left sidebar)
3. Under **"Source"**, select:
   - Branch: **main**
   - Folder: **/ (root)**
4. Click **"Save"**
5. Wait 2-3 minutes for deployment

### Step 5: Access Your Live Website! 🎉

Your app will be live at:
```
https://YOUR-USERNAME.github.io/REPO-NAME/Index-Clean.html
```

For example, if your username is `john-doe` and repo is `ssc-vocabulary`:
```
https://john-doe.github.io/ssc-vocabulary/Index-Clean.html
```

## 📁 Files to Upload

Make sure you upload these files:

```
your-repo/
├── Index-Clean.html       ⭐ Main app (REQUIRED)
├── vocab.html            ⭐ Vocabulary data (REQUIRED)
├── README.md             📝 Project description (optional but recommended)
├── QUICK_START.md        📝 Quick guide (optional)
└── vocab-data-loader.js  🔧 Standalone loader (optional)
```

**Minimum required:** Just `Index-Clean.html` and `vocab.html`

## 🔧 Optional: Rename Index-Clean.html to index.html

If you want a cleaner URL like:
```
https://YOUR-USERNAME.github.io/ssc-vocabulary/
```

Instead of:
```
https://YOUR-USERNAME.github.io/ssc-vocabulary/Index-Clean.html
```

Just rename `Index-Clean.html` to `index.html` before uploading!

## ✏️ How to Update Vocabulary Later

### Method 1: GitHub Web Interface
1. Go to your repository
2. Click on `vocab.html`
3. Click the pencil ✏️ icon (Edit)
4. Make your changes
5. Scroll down and click **"Commit changes"**
6. Your website updates automatically in 1-2 minutes!

### Method 2: Git Command Line
```bash
# Edit vocab.html locally
# Then:
git add vocab.html
git commit -m "Updated vocabulary"
git push
```

## 🎨 Customize Your Repository

### Add a Nice README

Create a `README.md` file in your repo with:

```markdown
# SSC Vocabulary Flashcards

Interactive flashcard application for SSC exam preparation.

## 🌐 Live Demo
https://YOUR-USERNAME.github.io/ssc-vocabulary/Index-Clean.html

## ✨ Features
- 957+ vocabulary words
- Multiple SSC exams (CGL, CHSL, MTS, CPO, GD, Steno, JE)
- Flashcard mode with flip animation
- Quiz mode with scoring
- Progress tracking
- Mobile-friendly design

## 📚 Exam Coverage
- SSC CGL (Combined Graduate Level)
- SSC CHSL (10+2 Level)
- SSC MTS (Multi Tasking Staff)
- SSC CPO (Central Police Organisation)
- SSC GD (General Duty)
- SSC Stenographer
- SSC JE (Junior Engineer)

## 🚀 Usage
Simply visit the live link and start studying!

## 📝 Adding New Words
Edit `vocab.html` and add new words following the template provided.

## 📄 License
Free to use for educational purposes.
```

## ❓ Troubleshooting

### "Page not found" after enabling GitHub Pages
- Wait 3-5 minutes for deployment
- Check the exact URL (case-sensitive)
- Make sure files are in the root folder

### Vocabulary not loading
- Both `Index-Clean.html` and `vocab.html` must be in the same folder
- File names are case-sensitive
- Clear browser cache (Ctrl+Shift+R)

### Changes not showing up
- Wait 1-2 minutes for GitHub to rebuild
- Clear browser cache
- Check if commit was successful

## 🎁 Bonus: Custom Domain (Optional)

Want a custom domain like `ssc-vocab.com`?

1. Buy a domain from Namecheap, GoDaddy, etc.
2. In your repo **Settings** → **Pages** → **Custom domain**
3. Enter your domain
4. Follow GitHub's DNS configuration guide

## 📧 Need Help?

- GitHub Pages Documentation: https://pages.github.com
- GitHub Guides: https://guides.github.com
- Ask in GitHub Community: https://github.community

---

**That's it! Your SSC Vocabulary app will be live on the internet for free!** 🎉
