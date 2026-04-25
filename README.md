# DispatchPro
### Laminate Order Management SaaS — by AppCentrik

A mobile-first PWA for managing laminate orders from creation to dispatch.

## Roles
- **Super Admin** — AppCentrik (you) — manage all tenants
- **Admin** — Business owner — manage users, view reports
- **Office Staff** — Create orders
- **Godown Manager** — Accept & dispatch orders
- **Godown Floor** — Pack orders, mark ready

## Tech Stack
- Firebase Auth + Firestore
- Vanilla JS PWA (single file)
- GitHub Pages hosting

## Setup
1. Push to GitHub repo
2. Enable GitHub Pages (root, main branch)
3. Add custom domain in repo settings
4. Create super admin in Firebase Auth console + Firestore `users` collection

## First Login Setup (Firebase Console)
1. Firebase Auth → Add user (your email + password)
2. Firestore → `users` collection → New doc with your UID:
   - name: "Rahul"
   - email: "your@email.com"
   - role: "superadmin"
   - tenantId: ""
   - tenantName: "AppCentrik"
3. Login → Create first tenant → Add users

## Domain
Hosted at: dispatchpro.appcentrik.in (or per-client subdomains)
