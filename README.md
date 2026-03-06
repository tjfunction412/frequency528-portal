# Frequency 528 — Growth Initiative Portal

Professional client portal and investor brief for Frequency 528's growth strategy.

**Live URL:** https://frequency528-portal.vercel.app

---

## Repository Access

**GitHub Repository:** `tjfunction412/frequency528-portal`

**GitHub Username:** `tjfunction412`

**GitHub Token (for CLI access):** `[Ask TJ for token — stored securely outside repo]`

---

## Project Structure

```
frequency528-portal/
├── index.html                              # Main portal page (light mode, professional)
├── logo.png                                # Frequency 528 branding logo
├── Frequency_528_Growth_Initiative.pdf     # One-page investor brief (printable)
├── vercel.json                             # Vercel deployment config
├── README.md                               # This file
└── .git/                                   # Git repository
```

---

## What's Included

### 1. **Interactive Portal** (`index.html`)
- Clean, light-mode design
- 5-phase strategy breakdown with clickable expandable sections
- Responsive mobile design
- Professional branding with logo
- PDF download button

### 2. **One-Page Investor Brief** (PDF)
- Condensed strategic summary
- Key metrics and timeline front-and-center
- Professional tone (no hype)
- Function Consulting LLC footnote (credible, minimal ego)
- Print-ready formatting

### 3. **Live Deployment** (Vercel)
- Auto-deploys from GitHub `main` branch
- Live URL: `https://frequency528-portal.vercel.app`
- No build step required (static HTML)

---

## Making Future Changes

### Option 1: Update Locally & Push (Recommended)

1. Clone the repo:
```bash
git clone https://github.com/tjfunction412/frequency528-portal.git
cd frequency528-portal
```

2. Edit files (e.g., `index.html`, `logo.png`)

3. Commit and push:
```bash
git add .
git commit -m "Description of changes"
git push origin main
```

4. Vercel auto-redeploys (30 seconds)

### Option 2: Ask Claude to Update

Share this README with Claude in a future window. Claude can:
- Push directly to GitHub using the token above
- Update HTML content, phases, metrics, branding
- Regenerate the PDF
- Deploy changes

**Just paste the token when asked — it's safe to reuse.**

---

## Making Edits to the Portal

### HTML Content (index.html)
- **Hero section:** Logo, title, tagline (lines 250–260)
- **Executive Overview:** Key metrics, strategic pivot (lines 270–320)
- **Phase Details:** All phase content is expandable (lines 400+)
- **Colors/Styling:** All CSS is in `<style>` tag at top (lines 7–250)

### PDF Content
The PDF is auto-generated from a Python script. To regenerate after HTML changes:
```bash
python /path/to/generate_onepager.py
```

### Logo
Replace `logo.png` with new file. Must be PNG with white/transparent background for light theme.

---

## Deployment Details

**Platform:** Vercel  
**Domain:** `frequency528-portal.vercel.app`  
**Branch:** `main`  
**Auto-deploy:** Enabled (deploys on every push to `main`)  

To manually redeploy:
1. Go to https://vercel.com/dashboard
2. Select `frequency528-portal` project
3. Click "Deployments" → "Redeploy" on latest build

---

## Customization Tips

### Change Colors
Edit CSS variables in `index.html`:
```css
:root {
    --accent: #0066cc;        /* Change this for primary color */
    --bg-primary: #ffffff;    /* Background */
    --text-primary: #1a1a1a;  /* Text */
}
```

### Add More Phases
Copy a phase card in the roadmap section and duplicate the phase-detail section below.

### Update Metrics
Find the summary cards in the Executive Overview section — update values in `.summary-card` divs.

---

## Troubleshooting

**Portal not updating after push?**
- Wait 30 seconds for Vercel to redeploy
- Hard refresh browser: `Cmd+Shift+R` (Mac) or `Ctrl+Shift+R` (Windows)
- Check Vercel dashboard to confirm deployment succeeded

**PDF not downloading?**
- Ensure `Frequency_528_Growth_Initiative.pdf` exists in repo root
- Commit and push if you regenerated it
- Check Vercel deployment includes the PDF file

**Logo not showing?**
- Logo file must be in repo root as `logo.png`
- Must be PNG format with white or transparent background
- Check HTML line ~250 for correct path: `src="./logo.png"`

---

## Contact & Support

**Repository Owner:** TJ (tjfunction412)  
**Business:** Function Consulting LLC  
**Client:** Frequency 528 (Ryan)  
**Live Portal:** https://frequency528-portal.vercel.app

---

## Version History

**v1.0** (March 2026)
- Initial portal launch with 5-phase strategy
- Interactive phase cards with expandable details
- Professional one-page PDF brief
- Live on Vercel with auto-deploy from GitHub

---

*Last Updated: March 6, 2026*
