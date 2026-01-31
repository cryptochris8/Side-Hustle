# Project Template - Quick Start Guide

Use this template for every Side Hustle project to enforce shipping rules.

---

## Before You Start

1. Read SHIPPING-RULES.md
2. Set a 7-day deadline (put it in your calendar)
3. Define your 3 core features (no more!)

---

## Project Setup Checklist

### Day 1: Research & Planning (4 hours max)

- [ ] Identify the problem
- [ ] Talk to 3 potential users (friends, Reddit, Twitter)
- [ ] Validate they'd pay for a solution
- [ ] Define 3 core features only
- [ ] Choose your tech stack (from approved list below)

### Day 2-3: Build Core Feature (16 hours max)

- [ ] Set up project with template/boilerplate
- [ ] Build feature #1
- [ ] Build feature #2
- [ ] Build feature #3
- [ ] Basic styling (copy/paste components)

### Day 4: Auth + Payment (8 hours max)

- [ ] Add authentication (Supabase/Clerk/etc)
- [ ] Add payment method (Stripe link minimum)
- [ ] Create simple landing page

### Day 5: Deploy + Test (8 hours max)

- [ ] Deploy to Vercel/Netlify/Railway
- [ ] Test happy path (main user flow)
- [ ] Fix critical bugs only

### Day 6: Final Polish (4 hours max)

- [ ] Fix any deployment issues
- [ ] Test payment flow
- [ ] Write basic instructions

### Day 7: Launch (4 hours max)

- [ ] Post on Reddit/Twitter/relevant communities
- [ ] Email/message potential users
- [ ] Set up basic analytics (Google Analytics or similar)

**SHIP BY END OF DAY 7. NO EXCEPTIONS.**

---

## Approved Tech Stacks (Pick One, Don't Mix)

### Stack 1: Next.js Full-Stack (Recommended)
- **Framework**: Next.js 14+ (App Router)
- **Database**: Supabase (includes auth)
- **Styling**: Tailwind CSS + shadcn/ui
- **Hosting**: Vercel
- **Payments**: Stripe
- **Why**: One framework, fast deployment, great DX

### Stack 2: Simple Node/Express
- **Backend**: Express.js
- **Frontend**: HTML + Tailwind CSS
- **Database**: Supabase or Firebase
- **Auth**: Clerk or Firebase Auth
- **Hosting**: Railway or Render
- **Payments**: Stripe
- **Why**: Simple, familiar, less magic

### Stack 3: Python Flask (If you prefer Python)
- **Backend**: Flask
- **Frontend**: Jinja2 templates + Tailwind
- **Database**: Supabase or SQLite
- **Auth**: Flask-Login or Auth0
- **Hosting**: Railway or Render
- **Payments**: Stripe
- **Why**: Python is easy, Flask is minimal

### Stack 4: No-Code/Low-Code First
- **Frontend**: Carrd or Webflow
- **Backend**: Make.com or Zapier
- **Database**: Airtable or Google Sheets
- **Auth**: Memberstack
- **Payments**: Gumroad or Stripe
- **Why**: Ship even faster, code only what you need

---

## Project Structure (Example: Next.js)

```
/project-name
├── /app
│   ├── /api              # API routes
│   ├── /dashboard        # User dashboard
│   ├── /auth             # Auth pages
│   └── page.tsx          # Landing page
├── /components           # Reusable components
├── /lib                  # Utilities
├── .env.local            # Environment variables
└── README.md
```

**Keep it simple. Don't over-organize in V1.**

---

## Feature Definition Template

Use this for every project:

### Project Name: [Your Project]

**Problem**: [One sentence describing the problem]

**Solution**: [One sentence describing your solution]

**Target User**: [Who will pay for this?]

**Pricing**: [How much? Start high, can always lower]

### V1 Features (MAX 3)

1. **Feature 1**: [Name]
   - **What it does**: [One sentence]
   - **Why it matters**: [Solves X problem]

2. **Feature 2**: [Name]
   - **What it does**: [One sentence]
   - **Why it matters**: [Solves X problem]

3. **Feature 3**: [Name]
   - **What it does**: [One sentence]
   - **Why it matters**: [Solves X problem]

### V2 Ideas (Do NOT build these in V1)

- [Feature idea 1]
- [Feature idea 2]
- [Feature idea 3]
- etc.

### Tech Stack

- Framework: [e.g., Next.js]
- Database: [e.g., Supabase]
- Auth: [e.g., Supabase Auth]
- Payments: [e.g., Stripe]
- Hosting: [e.g., Vercel]

### Launch Deadline

**Start Date**: [Date]
**Ship Date**: [Date - MAX 7 days later]

---

## Quick Start Commands

### Next.js Template
```bash
npx create-next-app@latest project-name
cd project-name
npm install @supabase/supabase-js
npx shadcn-ui@latest init
```

### Express Template
```bash
mkdir project-name && cd project-name
npm init -y
npm install express
```

### Flask Template
```bash
mkdir project-name && cd project-name
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
pip install flask
```

---

## Daily Standup (Do this every day)

Answer these questions:

1. **What did I ship yesterday?**
2. **What will I ship today?**
3. **Am I still on track for 7-day launch?**
4. **Am I adding features beyond the core 3?** (If yes, STOP)

---

## Red Flag Check

Before you code anything, ask:

- **Is this one of my 3 core features?** No → Don't build it
- **Can I use an existing service for this?** Yes → Use it
- **Will users pay me without this?** Yes → V2 feature
- **Am I doing this to make it "perfect"?** Yes → Stop

---

## Launch Checklist

Before you announce your project:

- [ ] Core feature works (test it yourself)
- [ ] Someone else can sign up and use it
- [ ] Payment method is working (test with real card)
- [ ] Site is live and accessible
- [ ] You have a way to contact users (email list minimum)

That's it. If you have all 5, you MUST launch.

---

## Post-Launch

### First 24 Hours
- Monitor for crashes
- Fix critical bugs only
- Respond to all user feedback
- Don't add new features yet

### First Week
- Collect feedback
- Track which features get used
- Ask users what they need most

### First Month
- Analyze usage data
- Plan V2 based on real user feedback
- Only then start building new features

---

## Remember

You're not building a unicorn startup. You're building a side hustle that generates revenue.

**Shipped and imperfect > Perfect and hidden**

NOW GO BUILD SOMETHING AND SHIP IT.
