# KJS Accounting — Free Consultation Contact Form

Professional contact form for KJS Accounting's free consultation inquiries.

**Live:** https://tmoneysurvey.github.io/kjs-contact-form/

---

## About

Contact form captures:
- Full Name
- Email Address
- Phone Number
- Account Type (Business / Personal)
- Interest in Free Consultation (checkbox)
- Additional Details (optional)

Submissions sent via **FormSubmit.co** to KJS Accounting's configured email.

---

## Tech Stack

- **HTML5** with form validation
- **CSS3** with responsive design
- **FormSubmit.co** for backend email processing
- **GitHub Pages** for hosting

---

## Features

✅ Responsive mobile/tablet/desktop design  
✅ Email validation (HTML5)  
✅ Auto-response emails to submitters  
✅ Form submission via FormSubmit.co  
✅ Professional styling (dark theme + cyan-purple gradient)  
✅ "Back to Home" navigation link  

---

## How It Works

1. Visitor fills out the form
2. Submits to FormSubmit.co
3. Receives auto-response email
4. KJS Accounting receives submission
5. Redirects to main Canva site

---

## Setup

No setup required — just host on GitHub Pages and link from your main site.

**Link from your Canva site to:**
```
https://tmoneysurvey.github.io/kjs-contact-form/
```

Or relative link if both files are in the same folder:
```html
<a href="contact.html">Free Consultation</a>
```

---

## Configuration

Email address for form submissions is configured in `contact.html` (line 184).

To update, edit the `action` attribute:
```html
<form action="https://formsubmit.co/EMAIL_HERE" method="POST">
```

---

## Customization

### Colors
- Gradient button: Lines 114-115 (cyan `#00c4cc` to purple `#7d2ae8`)
- Background: Line 16 (dark gradient)
- Text: Line 17 (dark gray `#333`)

### Form Fields
Edit lines 191-236 to add/remove fields. Each field follows the pattern:
```html
<div class="form-group">
    <label for="field-id">Label</label>
    <input type="text" id="field-id" name="field-name" required>
</div>
```

### Button Text
Line 239: Change "Request Consultation" to desired text

---

## Deployment

Push to `main` branch — auto-deploys to GitHub Pages within 1-2 minutes.

```bash
git add contact.html README.md
git commit -m "Initial commit: KJS contact form"
git push origin main
```

---

## Live Testing

1. Visit: https://tmoneysurvey.github.io/kjs-contact-form/
2. Fill out form
3. Submit
4. Check email for auto-response

---

## Support

Hosted on GitHub Pages. For issues:
- Check FormSubmit.co dashboard
- Verify email address in form action
- Test locally: `python3 -m http.server 8000`

---

**Repo:** https://github.com/tmoneysurvey/kjs-contact-form
