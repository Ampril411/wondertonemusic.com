# WonderTone Music Studio Website

## 📁 File Structure

```
wondertone/
├── index.html          ← Main website (all pages)
├── images/             ← All photos go here
│   ├── logo-black.jpg
│   ├── logo-white.jpg
│   ├── reception-bright.jpg
│   ├── piano-kawai.jpg
│   └── ... (all studio photos)
├── admin/
│   ├── index.html      ← CMS login page
│   └── config.yml      ← CMS configuration
└── README.md           ← This file
```

---

## ✏️ HOW TO EDIT CONTENT (Non-Technical)

### Option A: Simple direct edits in index.html

Search for these comment tags and edit the value below them:

| What to change | Search for |
|---|---|
| Email address | `<!-- EDIT: Replace with real email -->` |
| Phone number | `<!-- EDIT: Replace with real phone number -->` |
| Address | `<!-- EDIT: Replace with real address -->` |
| Business hours | `<!-- EDIT: Replace with real hours -->` |
| Google Maps | `<!-- EDIT: Replace with Google Maps embed iframe -->` |

To get a Google Maps embed:
1. Go to maps.google.com, find your location
2. Click Share → Embed a map → Copy HTML
3. Paste it replacing the `<div class="map-placeholder">` section

### Option B: Free CMS admin panel (recommended after deployment)

After deployment, visit `yoursite.com/admin` to manage:
- 📷 Gallery photos (upload, reorder, caption)
- 💬 Testimonials (add/edit parent reviews)
- 📚 Programs (add/edit course descriptions)
- 👩‍🏫 Teacher profiles
- ⚙️ Studio info (contact, hours, stats)

---

## 🚀 FREE DEPLOYMENT (GitHub Pages + Netlify)

Your technical friend needs to do this once — takes about 1–2 hours.

### Step 1: Create GitHub account
- Go to github.com and create a free account
- Create a new repository named `wondertone-website`
- Upload all files from this folder

### Step 2: Deploy via Netlify (free)
1. Go to netlify.com → "Add new site" → "Import from Git"
2. Connect to GitHub, select `wondertone-website`
3. Click Deploy — site goes live at a random URL (e.g. `random-name.netlify.app`)
4. To use custom domain: "Domain settings" → Add `wondertonemusic.com`

### Step 3: Enable CMS editing (Decap CMS)
1. In Netlify dashboard → "Integrations" → "Identity" → Enable
2. Go to "Identity" → "Settings" → "Git Gateway" → Enable
3. Invite Ariel/Jimmy at "Identity" → "Invite users"
4. Visit `yoursite.com/admin` to log in with the invite link

### Custom domain
- Buy `wondertonemusic.com` at namecheap.com (~$12/year)
- In Netlify: Domain Settings → Add custom domain → Follow DNS instructions

---

## 📸 REPLACING PHOTOS

### Option 1: Via CMS (after setup)
- Login at yoursite.com/admin → Gallery → Upload photos

### Option 2: Direct file replacement
- Replace any file in the `images/` folder with same filename
- Commit & push to GitHub → Netlify auto-redeploys in ~1 min

### Recommended photo sizes
- Hero/wide photos: 1600×1000px minimum
- Portrait photos: 800×1000px minimum
- All formats: JPG preferred (smaller file size)

---

## 📋 FUTURE ADDITIONS (Phase 2)

When you're ready to add these features:
- **Blog / News** — Netlify + Decap CMS supports this natively
- **Online booking** — Add Calendly embed (free) or Acuity ($)
- **Student portal** — Requires backend work
- **WeChat QR code** — Add to contact section

---

## 🆘 QUICK HELP

**Text looks wrong?** Open index.html in a text editor, use Ctrl+F to find the text, edit it.

**Photo not showing?** Make sure filename matches exactly (case-sensitive on servers).

**Form not sending emails?** Need to connect to Netlify Forms or Formspree — see tech friend.

For content questions: Edit index.html
For deployment issues: Ask your technical friend
For design changes: Contact Claude (save your conversation link)
