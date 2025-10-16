# 🚀 GitHub Deployment Guide for Snail gram

## 📦 What You Need

- GitHub account (free)
- The files: `index.html` and `README.md`
- 5 minutes

---

## 🎯 Method 1: GitHub Web Interface (No Code, Easiest!)

### Step 1: Create Repository

1. Go to [github.com](https://github.com)
2. Click the **"+"** icon (top right) → **"New repository"**
3. Fill in:
   - **Repository name**: `snailgram`
   - **Description**: "Social media at a snail's pace 🐌"
   - **Public** (check this)
   - **Add a README**: Leave UNCHECKED
4. Click **"Create repository"**

### Step 2: Upload Files

1. On your new repo page, click **"uploading an existing file"**
2. Drag and drop:
   - `index.html`
   - `README.md`
3. Scroll down, click **"Commit changes"**

### Step 3: Enable GitHub Pages

1. Go to **Settings** (top right)
2. Scroll down to **"Pages"** (left sidebar)
3. Under **"Source"**, select:
   - Branch: **main**
   - Folder: **/ (root)**
4. Click **"Save"**
5. Wait 1-2 minutes

### Step 4: Get Your URL

After a minute, refresh the Pages settings.

You'll see: **"Your site is live at https://YOUR_USERNAME.github.io/snailgram"**

**Copy that URL and open it on your phone!** 📱

---

## 🎯 Method 2: Using Git (Command Line)

### Prerequisites:
```bash
# Install Git first if you don't have it
# Mac: comes pre-installed
# Windows: download from git-scm.com
```

### Step 1: Initialize Repository

```bash
# Navigate to the folder with your files
cd path/to/snailgram

# Initialize git
git init

# Add files
git add index.html README.md

# Commit
git commit -m "Initial commit - Snail gram 🐌"
```

### Step 2: Create GitHub Repo

1. Go to github.com → New repository
2. Name it `snailgram`
3. Keep it public
4. **DON'T** initialize with README
5. Click "Create repository"

### Step 3: Push to GitHub

GitHub will show you commands. Use these:

```bash
# Add remote
git remote add origin https://github.com/YOUR_USERNAME/snailgram.git

# Push
git branch -M main
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username!

### Step 4: Enable Pages

```bash
# Go to Settings → Pages on GitHub
# Set source to main branch
# Save
```

---

## 🎯 Method 3: GitHub Desktop (GUI)

### Step 1: Download GitHub Desktop

- Go to [desktop.github.com](https://desktop.github.com)
- Download and install
- Sign in with your GitHub account

### Step 2: Create Repository

1. File → **New Repository**
2. Name: `snailgram`
3. Local Path: Choose where to save
4. Click **"Create Repository"**

### Step 3: Add Files

1. Copy `index.html` and `README.md` into the folder
2. GitHub Desktop will show the changes
3. Write commit message: "Initial commit"
4. Click **"Commit to main"**

### Step 4: Publish

1. Click **"Publish repository"**
2. Uncheck "Keep this code private"
3. Click **"Publish repository"**

### Step 5: Enable Pages

1. Go to github.com/YOUR_USERNAME/snailgram
2. Settings → Pages
3. Source: main branch
4. Save

---

## ✅ Verification Checklist

After uploading, check:

- [ ] Repository is public
- [ ] `index.html` is in root folder (not in subfolder)
- [ ] `README.md` is in root folder
- [ ] GitHub Pages is enabled (Settings → Pages)
- [ ] URL works: `https://YOUR_USERNAME.github.io/snailgram`
- [ ] Open URL on mobile phone
- [ ] Tilt works, shake works, breathing works

---

## 🐛 Common Issues

### "404 - Page Not Found"

**Fix:**
- Wait 2-5 minutes (GitHub Pages takes time)
- Check file is named `index.html` (not `index.HTML`)
- Ensure Pages is enabled in Settings
- Refresh/clear cache

### "Page Shows Code Instead of App"

**Fix:**
- File must be named `index.html` exactly
- Check file is in root folder (not in `/docs` or subfolder)
- Re-enable Pages: Settings → Pages → Save again

### "Permission Denied" Error

**Fix:**
```bash
# If using SSH, switch to HTTPS:
git remote set-url origin https://github.com/YOUR_USERNAME/snailgram.git

# Then push again:
git push -u origin main
```

### "Sensors Don't Work"

**Fix:**
- GitHub Pages uses HTTPS automatically (good!)
- Make sure you're on mobile device
- Grant permissions when prompted
- Settings → Safari → Motion Access → ON

---

## 🔄 Updating Your Site

Made changes to `index.html`? Here's how to update:

### Via GitHub Web:

1. Go to your repo
2. Click on `index.html`
3. Click pencil icon (Edit)
4. Make changes
5. Scroll down, click "Commit changes"
6. Wait 1 minute, refresh your site

### Via Git:

```bash
# Make changes to index.html locally
# Then:
git add index.html
git commit -m "Updated feature X"
git push
```

---

## 🎨 Customization After Upload

### Change Videos:

1. Edit `index.html` on GitHub
2. Find the `videos` array
3. Replace URLs with your own
4. Commit changes

### Change Colors:

1. Edit the `<style>` section in `index.html`
2. Change hex colors (e.g., `#0095f6` to `#ff0000`)
3. Commit

---

## 📊 Get Stats (Optional)

Want to see how many people use it?

### Add Google Analytics:

1. Get tracking ID from [analytics.google.com](https://analytics.google.com)
2. Add this before `</head>` in `index.html`:

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

Replace `GA_MEASUREMENT_ID` with your actual ID.

---

## 🌟 Next Steps

### Share Your Work:

- Tweet the link with #Snailgram
- Add to your portfolio
- Submit to design showcases
- Show friends (watch them struggle)

### Make It Better:

- Add more videos
- Create custom animations
- Add more gesture types
- Translate to other languages

### Get Feedback:

- Enable Issues on your repo
- Ask friends to test
- Post on Reddit r/InternetIsBeautiful
- Submit to Product Hunt

---

## 📱 QR Code for Easy Sharing

Want a QR code?

1. Go to [qr-code-generator.com](https://www.qr-code-generator.com)
2. Enter your GitHub Pages URL
3. Download QR code
4. People can scan with their phones!

---

## 🎉 You're Done!

Your Snail gram is now live on the internet! 🌍

**Your URL:**  
`https://YOUR_USERNAME.github.io/snailgram`

**Share it everywhere and watch people get frustrated!** 😅🐌

---

## 🆘 Still Need Help?

1. Check [GitHub Pages docs](https://docs.github.com/en/pages)
2. Open an Issue on the original Snail gram repo
3. Google your specific error message
4. Ask on [Stack Overflow](https://stackoverflow.com) with tag `github-pages`

---

**Happy deploying! 🚀🐌**
