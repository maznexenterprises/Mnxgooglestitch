# Maznex Enterprises Ltd — Website (Vercel Deployment)

## 🚀 Deploy to Vercel in 3 Steps

### Option A: Vercel CLI (Fastest)
```bash
npm install -g vercel
cd maznex_vercel
vercel --prod
```

### Option B: Vercel Dashboard (No-code)
1. Go to [vercel.com](https://vercel.com) and sign in
2. Click **"Add New Project"**
3. Click **"Upload"** (drag & drop this folder)
4. Click **Deploy** — done!

### Option C: GitHub (Recommended for updates)
1. Create a new GitHub repository
2. Upload all files from this folder
3. Connect repo to Vercel → auto-deploys on every push

---

## 📄 Site Structure

| File | Page |
|------|------|
| `index.html` | Home Page |
| `services.html` | Financial Services |
| `recruitment.html` | Recruitment Division |
| `packages.html` | Financial Service Packages |
| `recruitment-packages.html` | Recruitment Packages |
| `contact.html` | Contact & FAQ |
| `insights.html` | Market Insights Blog |
| `jobs.html` | Job Search |
| `login.html` | Client Login Portal |
| `admin.html` | Admin Dashboard |
| `candidate-portal.html` | Candidate Dashboard |
| `employer-dashboard.html` | Employer Dashboard |
| `checkout-success.html` | Payment Confirmation |
| `404.html` | Not Found Page |

---

## ⚙️ After Deployment — What to Configure

### 1. Stripe Payments
Replace the Stripe placeholder keys in `packages.html` and `recruitment-packages.html`:
```
pk_test_XXXX → your live Stripe publishable key
```

### 2. Currency Exchange API
The site uses `open.er-api.com` for live exchange rates. No API key needed for basic use.

### 3. Contact Form
The contact form currently has no backend. Options:
- **Formspree** (free): Add `action="https://formspree.io/f/YOUR_ID"` to the form
- **Netlify Forms**: Works if hosted on Netlify instead
- **EmailJS**: Client-side email sending

### 4. Custom Domain
In Vercel dashboard → Project Settings → Domains → Add `maznex.co.uk` or `maznexenterprises.com`

### 5. Google Analytics
Add your GA4 tag before `</head>` in each page:
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
```

### 6. Logo
Replace the SVG text logo with your actual logo file:
- Upload your logo as `logo.png` or `logo.svg`
- Replace the `<svg>MX</svg>` block in each nav with `<img src="/logo.png" alt="Maznex">`

---

## 🎨 Brand Colours
- Gold: `#C9A84C`
- Black: `#1A1A1A`
- Navy: `#1B3A6B`
- White: `#FFFFFF`

## 📞 Contact
WhatsApp button is pre-configured to +44 7424 748791
