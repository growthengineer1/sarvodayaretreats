# Formspree Setup Instructions

Your contact form is ready to send emails! Just follow these simple steps:

## Step 1: Sign Up for Formspree

1. Go to **https://formspree.io**
2. Click "Get Started" or "Sign Up"
3. Choose the **Free plan** (50 submissions/month - perfect to start!)
4. Create your account

## Step 2: Create Your Form

1. Once logged in, click **"+ New Form"**
2. Enter your email: **sarvodayaretreats@gmail.com**
3. Give your form a name (e.g., "Sarvodaya Contact Form")
4. Click "Create Form"

## Step 3: Get Your Form Endpoint

1. After creating the form, you'll see your unique endpoint
2. It will look like: `https://formspree.io/f/xxxxxxxx`
3. **Copy this URL** - you'll need it in the next step

## Step 4: Update Your Website

1. Open `index.html` in your code editor
2. Find this line (around line 1055):
   ```html
   <form class="contact-form" id="contactForm" action="YOUR_FORMSPREE_ENDPOINT" method="POST">
   ```
3. Replace `YOUR_FORMSPREE_ENDPOINT` with your actual Formspree URL:
   ```html
   <form class="contact-form" id="contactForm" action="https://formspree.io/f/xxxxxxxx" method="POST">
   ```
4. Save the file

## Step 5: Deploy & Test

1. Push your updated `index.html` to GitHub
2. Wait for Cloudflare Pages to deploy (usually takes 1-2 minutes)
3. Visit your live website
4. Test the contact form by filling it out and submitting
5. Check **sarvodayaretreats@gmail.com** - you should receive the inquiry!

## What Happens Now?

When someone submits your contact form:
- ✅ Their message is sent to **sarvodayaretreats@gmail.com**
- ✅ They see a success message on your website
- ✅ The email includes all fields: Name, Email, Dates, Duration, and Message
- ✅ You can reply directly from your Gmail inbox

## Formspree Features (Free Plan)

- 50 submissions per month
- Email notifications to sarvodayaretreats@gmail.com
- Spam filtering built-in
- View all submissions in Formspree dashboard
- Export submissions as CSV

## Need More Submissions?

If you get more than 50 inquiries per month, you can upgrade to:
- **Gold Plan**: $10/month for 1,000 submissions
- **Platinum Plan**: Custom pricing for unlimited submissions

## Troubleshooting

**Form not working?**
- Make sure you replaced `YOUR_FORMSPREE_ENDPOINT` with your actual endpoint
- Check that your Formspree form is active in the dashboard
- Look for any error messages in the browser console

**Not receiving emails?**
- Check your spam/junk folder in Gmail
- Verify the email address in your Formspree form settings
- Make sure you confirmed your Formspree account email

**Need help?**
- Formspree has great docs: https://help.formspree.io
- Their support is very responsive!

---

That's it! Your contact form is now live and will send all inquiries directly to your Gmail. 🎉
