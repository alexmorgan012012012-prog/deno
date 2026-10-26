# RYVO Digital Agency — Master Full-Stack Platform

> **"We Build. We Automate. We Create."**  
> *Digital experiences engineered for growth.*  
> **Contact Phone**: +92 308 2436424  
> **Contact Email**: [alexmorgan012012012@gmail.com](mailto:alexmorgan012012012@gmail.com)  
> **Direct WhatsApp**: [https://wa.me/923082436424](https://wa.me/923082436424)

---

## 1. System Overview

**RYVO Digital Agency** is a multi-page, full-stack digital agency and freelancing platform engineered with **React, TypeScript, Vite, Tailwind CSS, Framer Motion**, and **Supabase (PostgreSQL + Auth + Storage)**.

The application features:
- **Interactive 3D particle hero canvas** with real-time mouse interaction and radiant orange glow.
- **26 Public Pages** with responsive design, dynamic search (`⌘K`), and brand consistency.
- **Dedicated Services Marketplace** with 35+ professional disciplines, real-time search, category filters, sorting, package tiers, and direct scoping triggers.
- **Portfolio & Interactive Case Studies** featuring interactive Before/After sliders, business metrics, deliverables checklist, and tech stack badges.
- **Interactive Custom Project Quote Builder & Cost Estimator** calculating live estimates and issuing proposals into the database.
- **Complete Client Dashboard Suite** with project lifecycle tracking across 10 distinct status stages (`new_request` to `archived`), milestone timeline, deliverable downloads, revision requests, live chat, printable/downloadable PDF invoices, and support tickets.
- **Complete Protected Admin Back-Office** with genuine database analytics, project lifecycle transitions, services CRUD, portfolio CMS, content CMS, lead inbox, financial invoicing, user management, and global site settings.
- **Dual-Mode Hybrid Engine**: Operates immediately out-of-the-box with persistent demo data and seamlessly switches to live Supabase once `VITE_SUPABASE_URL` and `VITE_SUPABASE_ANON_KEY` are provided.

---

## 2. Design System & Visual Hierarchy

- **Near-Black Background**: `#08090B`
- **Charcoal Panels**: `#111318`
- **Lighter Charcoal / Cards**: `#181B22` & `#14171E`
- **Electric Orange Accent**: `#FF6A2A` (Hover: `#FF7D42`, Glow: `rgba(255, 106, 42, 0.25)`)
- **Typography**: Space Grotesk (Editorial headings), Plus Jakarta Sans (Clean prose), JetBrains Mono (Technical badges)
- **Cinematic Lighting**: Radial orange ambient glows, glassmorphism (`backdrop-blur-xl`), and micro-interactions.

---

## 3. Page & Route Directory

### A. Public Pages
1. `/` — Home (3D Hero Canvas, Metrics Ticker, Client Marquee, Featured Disciplines, Selected Projects, 6-Step Methodology, Testimonials, Insights, Bottom CTA)
2. `/about` — About RYVO (Studio manifesto, 4 core pillars, global performance metrics)
3. `/story` — Our Story (Chronological origin timeline from founding to AI telephony era)
4. `/team` — Studio Team (Profiles for Alex Morgan, David Reynolds, Elena Rostova, Tariq Al-Mansoor, Sarah Chen, Julian Bennett)
5. `/services` — Services Marketplace (35+ services across 8 categories, search, sort, save toggle)
6. `/services/:slug` — Individual Service Detail Pages (Dedicated page for every service, package tiers, deliverables, FAQs, related services)
7. `/portfolio` — Portfolio (Grid/masonry layouts, category filters, search, featured badges)
8. `/portfolio/:slug` — Project Case Studies (Interactive Before/After slider, challenges, solutions, metrics, deliverables)
9. `/process` — Our Process (Interactive 6-phase engineering framework deep-dive)
10. `/pricing` — Pricing & Packages (Transparent tiers: Launchpad, Growth, Enterprise, plus modular add-ons)
11. `/quote` — Custom Project Quote Builder (Interactive dynamic cost estimator, scope scale, timeline selection, live calculation)
12. `/reviews` — Verified Client Reviews (5.0/5.0 verified reviews, filter by service)
13. `/faq` — Agency FAQs (Searchable categorized accordion with direct contact shortcuts)
14. `/blog` — Insights Blog (Editorial articles, search, category filters)
15. `/blog/:slug` — Blog Article Detail (Markdown content, author info, social share, related insights)
16. `/contact` — Contact Us (Enquiry form, click-to-call, WhatsApp direct, response time pledge)
17. `/consultation` — Book a Consultation (Interactive date/time slot picker, timezone selector, instant booking)
18. `/careers` — Careers & Collaboration (Open roles, perks, application modal)
19. `/partners` — Agency Partner Program (15% commission referral alliance, white-label capacity)
20. `/help` — Help Center (Knowledge base guides, search, ticket link)
21. `/privacy` — Privacy Policy (GDPR / CCPA compliant)
22. `/terms` — Terms & Conditions (IP ownership, milestone payments, governing law)
23. `/cookies` — Cookie Policy (Cookie categorization & preferences)
24. `/refund-policy` — Refund & Cancellation Policy (Milestone-based protection, deposit rules)
25. `/search` — Global Search Results (`/search?q=...`)
26. `*` — 404 Not Found Page (Sleek terminal aesthetic with return navigation)

### B. Authentication Pages
- `/login` — Secure Login (with 1-click Client & Admin fast demo switcher)
- `/signup` — Workspace Registration
- `/forgot-password` — Password Recovery Request
- `/reset-password` — Password Reset Confirmation

### C. Client Dashboard Suite (`/dashboard/*`)
- `/dashboard` — Overview (Live KPIs, active project trackers, recent invoices, messaging shortcuts)
- `/dashboard/projects` — My Projects (Filter by status, sprint progress bars)
- `/dashboard/projects/:id` — Project Sprint Workspace (10-step lifecycle pipeline, milestones, deliverable file downloads, revision requests)
- `/dashboard/new-request` — New Project Request Form (Multi-service selection, budget, timeline, brief)
- `/dashboard/messages` — Project Messaging (Real-time client/admin chat thread with auto-replies)
- `/dashboard/invoices` — Invoices & Billing (Printable/Downloadable PDF modal, instant "Pay Balance" simulation)
- `/dashboard/quotes` — Proposals & Quotations (Itemized technical scopes, approve/reject buttons)
- `/dashboard/consultations` — Scheduled Strategy Sessions (Google Meet links, reschedule/cancel)
- `/dashboard/support` — Priority Support Desk (Ticket creation, priority levels, reply thread)
- `/dashboard/settings` — Account Settings (Profile editing, avatar URL, password change, notification toggles)

### D. Admin Back-Office Suite (`/admin/*`)
- `/admin` — Analytics & Command (Revenue metrics, pipeline distribution charts, audit trail)
- `/admin/projects` — Project Lifecycle Management (10-step status transitions, milestone editor, deliverable upload)
- `/admin/services` — Services CRUD (Add/edit disciplines, starting prices, turnaround, publish toggle)
- `/admin/portfolio` — Portfolio CMS (Add/edit case studies, metrics, cover images, featured toggle)
- `/admin/content` — Content CMS (Testimonials CRUD, FAQs CRUD, Blog articles manager)
- `/admin/enquiries` — Lead Ingestion (Contact briefs inbox, consultation approval, CSV export)
- `/admin/invoices` — Billing & Invoices (Generate milestone invoices for projects, mark as paid)
- `/admin/users` — User & Role Governance (Search accounts, promote to Admin or demote to Client)
- `/admin/settings` — Agency Settings (Brand name, phone, email, WhatsApp, top banner, maintenance mode)

---

## 4. One-Click Demo Accounts

For immediate testing, use the top navbar role switcher or the credentials below:

| Role | Email | Password | Display Name | Organization |
|---|---|---|---|---|
| **Client** | `client@ryvo.agency` | `ryvo2026!` | Dr. Marcus Vance | Lumina Health Network |
| **Admin** | `admin@ryvo.agency` | `admin2026!` | Alex Morgan | RYVO Digital Agency |

---

## 5. Local Development Setup

### Prerequisites
- Node.js v18+ or v20+
- npm v9+

### Commands

```powershell
# 1. Install dependencies
npm --prefix ryvo install

# 2. Run local development server
npm run dev
# Or directly inside the ryvo directory:
cd ryvo
npm run dev

# 3. Build for production (TypeScript check + Vite bundle)
npm run build

# 4. Preview production build locally
npm run preview
```

The application will run at `http://localhost:5173`.

---

## 6. Supabase Database Configuration (Optional Live Sync)

The application includes a master SQL migration file ready to run:
`supabase/migrations/20261021_init_ryvo_schema.sql`

### Connecting Live Supabase:
1. Create a project at [supabase.com](https://supabase.com).
2. Go to the **SQL Editor** in your Supabase dashboard.
3. Paste the contents of `supabase/migrations/20261021_init_ryvo_schema.sql` and click **Run**.
4. In your project, copy `.env.example` to `.env`:
   ```env
   VITE_SUPABASE_URL=https://your-project.supabase.co
   VITE_SUPABASE_ANON_KEY=your-anon-public-key-here
   ```
5. Restart the Vite server (`npm run dev`). The application will now read and write directly to your live Supabase database!

---

## 7. Production Deployment (Vercel / Netlify)

### Deploying to Vercel:
1. Push this repository to GitHub.
2. In Vercel, click **Add New Project** and select the repository.
3. Set **Root Directory** to `ryvo`.
4. Build command: `npm run build`
5. Output directory: `dist`
6. Add environment variables if using Supabase (`VITE_SUPABASE_URL`, `VITE_SUPABASE_ANON_KEY`).
7. Click **Deploy**.

---

## 8. Backup & Data Protection

- All client files and messages use encrypted cloud storage.
- When live Supabase is connected, automated daily PostgreSQL WAL-based backups are enabled automatically on the Supabase infrastructure.
- Administrative audit logs record every sensitive transition, user role adjustment, and invoice settlement.
