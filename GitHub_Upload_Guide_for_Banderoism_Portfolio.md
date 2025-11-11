# GitHub Upload Guide for Banderoism Portfolio

This guide will walk you through uploading your portfolio website to GitHub and deploying it permanently using Netlify or Vercel.

---

## Step 1: Create a GitHub Account (if you don't have one)

1. Go to [github.com](https://github.com)
2. Click **Sign up**
3. Enter your email, create a password, and choose a username
4. Verify your email address
5. Complete the setup process

---

## Step 2: Create a New Repository

1. Log in to GitHub
2. Click the **+** icon in the top right corner
3. Select **New repository**
4. Fill in the details:
   - **Repository name:** `banderoism-portfolio`
   - **Description:** "Professional portfolio website for Frank Fernandez - Video Producer & Editor"
   - **Public** (so it can be deployed)
   - **Initialize this repository with:** Leave unchecked
5. Click **Create repository**

---

## Step 3: Upload Files to GitHub

You have two options:

### Option A: Using GitHub Web Interface (Easiest)

1. On your new repository page, click **Add file** → **Upload files**
2. Drag and drop all files from the `banderoism-portfolio` folder:
   - `index.html`
   - `css/styles.css`
   - `js/script.js`
   - `README.md`
   - `LICENSE`
   - `.gitignore`
3. Scroll down and click **Commit changes**
4. Add a commit message: "Initial commit: Portfolio website"
5. Click **Commit changes**

### Option B: Using Git Command Line (Recommended)

1. **Install Git** (if not already installed):
   - Windows: Download from [git-scm.com](https://git-scm.com)
   - Mac: `brew install git`
   - Linux: `sudo apt-get install git`

2. **Open Terminal/Command Prompt** and run:
   ```bash
   cd /path/to/banderoism-portfolio
   ```

3. **Add remote repository:**
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/banderoism-portfolio.git
   git branch -M main
   git push -u origin main
   ```
   
   Replace `YOUR_USERNAME` with your actual GitHub username.

4. **When prompted**, enter your GitHub username and password (or personal access token)

---

## Step 4: Deploy to Netlify (Recommended)

Netlify offers free hosting with automatic deployments every time you push to GitHub.

### Steps:

1. Go to [netlify.com](https://netlify.com)
2. Click **Sign up** and choose **Sign up with GitHub**
3. Authorize Netlify to access your GitHub account
4. Click **New site from Git**
5. Select **GitHub** as your Git provider
6. Find and select `banderoism-portfolio` repository
7. Configure build settings:
   - **Branch to deploy:** `main`
   - **Build command:** Leave empty (static site)
   - **Publish directory:** `.` (root directory)
8. Click **Deploy site**

**Your website will be live in seconds!** Netlify will give you a URL like:
```
https://your-site-name.netlify.app
```

### Connect Custom Domain (Optional):

1. In Netlify dashboard, go to **Domain settings**
2. Click **Add custom domain**
3. Enter your domain (e.g., `banderoism.com`)
4. Follow the DNS configuration instructions

---

## Step 5: Deploy to Vercel (Alternative)

If you prefer Vercel instead of Netlify:

1. Go to [vercel.com](https://vercel.com)
2. Click **Sign up** and choose **Continue with GitHub**
3. Authorize Vercel
4. Click **New Project**
5. Select your `banderoism-portfolio` repository
6. Click **Import**
7. Leave default settings and click **Deploy**

Your site will be live at:
```
https://banderoism-portfolio.vercel.app
```

---

## Step 6: Update Your Website

After deployment, you can make changes anytime:

1. **Edit files locally** (on your computer)
2. **Commit and push to GitHub:**
   ```bash
   git add .
   git commit -m "Update: [describe your changes]"
   git push
   ```
3. **Netlify/Vercel will automatically redeploy** your site

---

## Important: Configure Contact Form

Before launching, set up your contact form:

1. Go to [formspree.io](https://formspree.io)
2. Sign up with your email
3. Create a new form
4. Copy your Form ID
5. Edit `index.html` and find this line:
   ```html
   <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
6. Replace `YOUR_FORM_ID` with your actual ID
7. Commit and push the changes

---

## Customization Checklist

Before going live, update these items:

- [ ] Replace `frank@banderoism.com` with actual email
- [ ] Update Instagram URL in Contact section
- [ ] Update YouTube channel URL in Contact section
- [ ] Set up Formspree contact form
- [ ] Replace placeholder YouTube video IDs with real reel
- [ ] Add real project images and videos
- [ ] Update project titles and descriptions
- [ ] Test contact form submission
- [ ] Test all navigation links
- [ ] Test on mobile devices

---

## Troubleshooting

### Site shows 404 error
- Make sure `index.html` is in the root directory
- Check that all file paths in HTML are correct

### Styles not loading
- Verify `css/styles.css` path is correct in HTML
- Check browser console for errors (F12)

### Contact form not working
- Verify Formspree Form ID is correct
- Check that form method is POST
- Test submission and check Formspree dashboard

### Deployment not updating
- Wait a few minutes for Netlify/Vercel to rebuild
- Check deployment logs in the dashboard
- Clear browser cache (Ctrl+Shift+Delete)

---

## Next Steps

1. ✅ Create GitHub account
2. ✅ Create repository
3. ✅ Upload files
4. ✅ Deploy to Netlify or Vercel
5. ✅ Configure contact form
6. ✅ Customize content
7. ✅ Test everything
8. ✅ Share your portfolio!

---

## Support Resources

- **GitHub Help:** https://docs.github.com
- **Netlify Docs:** https://docs.netlify.com
- **Vercel Docs:** https://vercel.com/docs
- **Formspree Help:** https://formspree.io/help

---

**Your portfolio website is ready to go live! 🚀**
