# Museum Ticket Booking System

## Overview
Static HTML/JS museum ticketing app with role-based dashboards (Customer/Employee/Manager). Uses localStorage for demo auth. Separate Next.js app in `/clerk-nextjs/` with Clerk auth.

**Live Demo:** [GitHub Pages URL after deploy]

## Quick Start
1. **Static HTML (root):** Open `login.html` in browser.
2. **Next.js:** `cd clerk-nextjs && npm install && npm run dev`

## Demo Credentials
- **Customer:** Register new or use any email/pass (stored localStorage)
- **Employee:** `employee@museum.com` / `employee123` or `EMP001`
- **Manager:** `manager@museum.com` / `manager123` or `MGR001`

## Deployment
### Static HTML (GitHub Pages)
- Push to GitHub, enable Pages on `main` branch → serves root HTML files.

### Next.js (Static Export or Vercel)
- Static: `cd clerk-nextjs && npm run build` → `out/` folder for GH Pages/docs.
- Vercel: Connect repo, auto-deploys.

## Project Structure
```
├── login.html, register.html, *-dashboard.html (static)
├── faq.html, customer-support.html
└── clerk-nextjs/ (Next.js + Clerk auth prototype)
```

Built with TailwindCSS, FontAwesome. No backend needed for demo.
