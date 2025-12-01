# 📧 Email Setup Guide - Contact Form

Your contact form is now configured to send emails to: **anassbenzina11@gmail.com**

## 🚀 Quick Setup (Choose One Method)

### Method 1: EmailJS (Recommended - Free & Easy)

1. **Sign up for EmailJS** (Free):
   - Go to: https://www.emailjs.com/
   - Click "Sign Up" and create a free account

2. **Create an Email Service**:
   - Go to "Email Services" in your dashboard
   - Click "Add New Service"
   - Choose "Gmail" (or your email provider)
   - Connect your Gmail account (anassbenzina11@gmail.com)
   - Copy your **Service ID**

3. **Create an Email Template**:
   - Go to "Email Templates"
   - Click "Create New Template"
   - Use this template:
     ```
     Subject: {{subject}}
     
     From: {{from_name}} ({{from_email}})
     
     Message:
     {{message}}
     
     Reply to: {{reply_to}}
     ```
   - Set "To Email" to: `anassbenzina11@gmail.com`
   - Copy your **Template ID**

4. **Get Your Public Key**:
   - Go to "Account" → "General"
   - Copy your **Public Key**

5. **Update the Code**:
   - Open `script.js`
   - Find these lines and replace:
     ```javascript
     emailjs.init("YOUR_PUBLIC_KEY"); // Replace with your Public Key
     ```
     ```javascript
     emailjs.send('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', { // Replace both IDs
     ```

### Method 2: Formspree (Even Easier - No Code Changes Needed)

1. Go to: https://formspree.io/
2. Sign up for a free account
3. Create a new form
4. Copy your form endpoint URL
5. Replace the EmailJS code in `script.js` with a simple fetch request

### Method 3: Simple Mailto (Basic Solution)

If you want a simple solution without setup, I can change the form to use mailto links (opens email client).

---

## ✅ After Setup

Once you've configured EmailJS:
1. Save all files
2. Refresh your browser
3. Test the contact form
4. Check your email inbox (anassbenzina11@gmail.com)

## 🆘 Need Help?

- EmailJS Documentation: https://www.emailjs.com/docs/
- Free tier allows 200 emails/month
- No backend server needed!

---

**Current Configuration:**
- Recipient Email: anassbenzina11@gmail.com
- Form Fields: Name, Email, Subject, Message


