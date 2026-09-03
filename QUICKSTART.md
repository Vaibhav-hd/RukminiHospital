# ⚡ Quick Start Guide - Rukmini Hospital Website

Get your hospital website live in **5 minutes**!

## 🎯 Quick Steps

### Step 1: Create GitHub Account (If you don't have one)
- Go to [github.com](https://github.com)
- Click **Sign up**
- Complete registration

### Step 2: Create New Repository
1. Click the **+** icon (top right) → **New repository**
2. Name: `rukmini-hospital`
3. Choose **Public**
4. Click **Create repository**

### Step 3: Upload Files
1. Click **Add file** → **Upload files**
2. Drag and drop these files:
   - `index.html`
   - `thankyou.html`
   - `logo.png`
   - `doctor.jpg`
   - `README.md`
   - `.gitignore`
3. Click **Commit changes**

### Step 4: Enable GitHub Pages
1. Go to **Settings** tab
2. Click **Pages** (left sidebar)
3. Under "Source" → Select **main** branch
4. Click **Save**
5. Wait 1-2 minutes ⏳

### Step 5: Access Your Website
Your site is now live at:
```
https://YOUR-USERNAME.github.io/rukmini-hospital/
```

---

## 📝 Important Changes to Make

### 1. **Update Email Address**
Open `index.html` and find this line:
```html
<form action="https://formsubmit.co/vaikunthviewdoc@gmail.com" method="POST">
```
Replace with your email.

### 2. **Update Phone Number** (Optional)
Search for `918669369486` and replace with your actual phone number (with country code, no + sign)

### 3. **Update Instagram Handle** (Optional)
Search for `dr.infin_ite24` and replace with your Instagram username

---

## 🖼️ Update Images

Your images should be in the root folder:
- `logo.png` - Hospital logo (current size: 2.1MB)
- `doctor.jpg` - Doctor's photo (current size: 644KB)

To replace:
1. Delete old files from GitHub
2. Upload new ones with same names

---

## ✅ What's Included

✨ **Features:**
- ✅ Fully responsive design (mobile, tablet, desktop)
- ✅ Beautiful animations and gradients
- ✅ Appointment booking form with validation
- ✅ Social media integration (WhatsApp, Instagram, Email)
- ✅ Doctor profile section
- ✅ Services showcase
- ✅ Contact form with Google Maps
- ✅ Thank you confirmation page

---

## 🎨 Customize Colors

Want to change the green and blue colors?

1. Open `index.html` in a text editor
2. Find the `<style>` section
3. Replace all instances:
   - `#0b7a5c` → Your primary color (green)
   - `#0f4c81` → Your secondary color (blue)

Example:
```css
/* Old */
background: #0b7a5c;

/* New */
background: #ff6b6b;  /* Your color */
```

---

## 📱 Test on Mobile

1. Open your site: `https://YOUR-USERNAME.github.io/rukmini-hospital/`
2. On mobile phone, test:
   - ✅ Menu opens/closes
   - ✅ Buttons work
   - ✅ Form submits
   - ✅ WhatsApp link opens
   - ✅ Call button dials

---

## 🚀 Extra Features Available

### Add Google Analytics
Track visitor data - Add this in `<head>`:
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-XXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'UA-XXXXXXX');
</script>
```

### Add Favicon
Create a small icon and upload as `favicon.ico`, then add:
```html
<link rel="icon" href="favicon.ico" type="image/x-icon">
```

### Add WhatsApp Chat Widget
Replace form with embedded chat - contact support for code

---

## 🆘 Troubleshooting

| Problem | Solution |
|---------|----------|
| **Form not sending** | Check email in form action tag |
| **Images not showing** | Verify filenames match exactly |
| **Site not loading** | Wait 5 minutes, then refresh |
| **Mobile menu broken** | Check browser console, clear cache |
| **Styles look weird** | Hard refresh: `Ctrl+Shift+R` (Windows) or `Cmd+Shift+R` (Mac) |

---

## 📞 Contact Details Update

Update these in the HTML:

**Phone:**
```html
<a href="tel:+918669369486">+91 8669369486</a>
```

**WhatsApp:**
```html
<a href="https://wa.me/918669369486">WhatsApp</a>
```

**Instagram:**
```html
<a href="https://instagram.com/dr.infin_ite24">Instagram</a>
```

**Email:**
```html
<a href="mailto:vaikunthviewdoc@gmail.com">Email</a>
```

---

## 🎯 Next Steps After Going Live

1. ✅ Test all links and buttons
2. ✅ Share website URL on social media
3. ✅ Add to Google Business Profile
4. ✅ Share WhatsApp link with patients
5. ✅ Monitor appointment submissions
6. ✅ Gather feedback and iterate

---

## 💡 Pro Tips

- 📱 **Mobile First**: Always test on mobile
- 🔗 **Share Direct Links**: Use short URLs for sharing
- 📊 **Track Submissions**: Check email for appointment forms
- 🎯 **Update Regularly**: Add news, testimonials, new services
- 💬 **Engage**: Respond to WhatsApp and email quickly

---

## 🔗 Useful Links

| Resource | URL |
|----------|-----|
| GitHub Pages Docs | https://pages.github.com/ |
| FormSubmit.co | https://formsubmit.co/ |
| Font Awesome Icons | https://fontawesome.com/icons |
| Google Fonts | https://fonts.google.com/ |
| Color Picker | https://htmlcolorcodes.com/ |

---

## 🚀 Deploy Code Updates

After making changes to your website:

```bash
git add .
git commit -m "Update website content"
git push origin main
```

Your changes will be live in **1-2 minutes**!

---

## 📊 Monitor Performance

Check your site speed:
- [PageSpeed Insights](https://pagespeed.web.dev/)
- [Google Lighthouse](https://developers.google.com/web/tools/lighthouse)
- [GTmetrix](https://gtmetrix.com/)

---

## 🎉 You're All Set!

Your professional hospital website is now **LIVE**! 

**Share your URL:**
```
https://YOUR-USERNAME.github.io/rukmini-hospital/
```

---

## 📞 Need Help?

- **GitHub Support**: https://support.github.com/
- **FormSubmit Issues**: https://formsubmit.co/support
- **Contact Doctor**: +91 8669369486

---

**Happy deploying! 🚀**

Created for Rukmini Hospital
Version: 2.0
