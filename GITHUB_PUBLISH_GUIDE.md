# Publishing Sarvodaya Retreats to GitHub + Cloudflare

Follow these simple steps to get your website live on the internet!

## Step 1: Create a GitHub Account (if you don't have one)

1. Go to **https://github.com**
2. Click "Sign up"
3. Follow the steps to create your free account
4. Verify your email address

## Step 2: Create a New Repository

1. Once logged in, click the **"+"** icon in the top-right corner
2. Select **"New repository"**
3. Name it: `sarvodaya-retreats` (or any name you prefer)
4. **Important**: Make it **Public** (required for free Cloudflare hosting)
5. Do **NOT** check "Add a README file" (we already have one)
6. Click **"Create repository"**

## Step 3: Upload Your Files to GitHub

You'll see a page with instructions. Choose the **easiest method**:

### Method A: Upload Files Directly (Easiest - No Command Line)

1. On the repository page, click **"uploading an existing file"** link
2. Drag and drop ALL these files from your project:
   - `index.html`
   - `README.md`
   - `FORMSPREE_SETUP.md`
   - `.gitignore`
3. Scroll down and click **"Commit changes"**
4. Done! Your files are on GitHub.

### Method B: Using Git Commands (If you know Git)

From your terminal in this project folder:

```bash
git init
git add .
git commit -m "Initial commit - Sarvodaya Retreats website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/sarvodaya-retreats.git
git push -u origin main
```

(Replace `YOUR-USERNAME` with your actual GitHub username)

## Step 4: Deploy to Cloudflare Pages

Now let's make your website live!

1. Go to **https://pages.cloudflare.com**
2. Click **"Sign up"** (or log in if you have an account)
3. Create your free Cloudflare account
4. Once logged in, click **"Create a project"**
5. Click **"Connect to Git"**
6. Choose **"GitHub"** and authorize Cloudflare to access your repos
7. Select your **sarvodaya-retreats** repository
8. Configure the build settings:
   - **Project name**: sarvodaya-retreats (or customize it)
   - **Production branch**: main
   - **Build command**: Leave empty (no build needed!)
   - **Build output directory**: `/` (just a forward slash)
9. Click **"Save and Deploy"**

## Step 5: Wait for Deployment (1-2 minutes)

Cloudflare will now deploy your website. You'll see:
- "Initializing build environment" ✅
- "Deploying to Cloudflare's global network" ✅
- "Success! Your site is live" 🎉

## Step 6: Your Website is Live! 🌟

Once deployed, you'll get a URL like:
```
https://sarvodaya-retreats.pages.dev
```

**Your website is now live on the internet!**

## Step 7: Set Up Formspree (Don't Forget!)

Your contact form won't work yet. Follow the instructions in `FORMSPREE_SETUP.md`:

1. Sign up at formspree.io
2. Create a form for sarvodayaretreats@gmail.com
3. Get your endpoint URL
4. Update `index.html` (line 1055) with your Formspree endpoint
5. Push the change to GitHub (Cloudflare will auto-deploy)

## Optional: Add a Custom Domain

Want `sarvodayaretreats.com` instead of `.pages.dev`?

1. Buy your domain from Namecheap, GoDaddy, or any registrar
2. In Cloudflare Pages, go to your project settings
3. Click **"Custom domains"**
4. Click **"Set up a custom domain"**
5. Follow the instructions to point your domain to Cloudflare

## Updating Your Website Later

Whenever you want to make changes:

1. Edit your files (locally or on GitHub)
2. Commit and push to GitHub
3. Cloudflare automatically deploys the updates (usually within 1-2 minutes)

## Need Help?

- **GitHub Issues**: Check GitHub's help docs
- **Cloudflare Support**: https://developers.cloudflare.com/pages
- **Formspree Help**: https://help.formspree.io

---

## Your Website is Ready! 🎉

You now have a beautiful, professional website for Sarvodaya Retreats that:
- ✅ Loads super fast (thanks to Cloudflare's global CDN)
- ✅ Works on all devices (mobile, tablet, desktop)
- ✅ Has a working contact form (after Formspree setup)
- ✅ Looks artistic and authentic
- ✅ Is completely free to host!

Congratulations on launching your retreat space website! 🌿
