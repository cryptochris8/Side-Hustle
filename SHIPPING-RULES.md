# SHIPPING RULES - Anti-Perfectionism Framework

## Purpose
This document exists to prevent perfectionism from killing your side hustle. Read this EVERY TIME you start working on a project.

---

## The Problem
You tend to take too long to publish apps because you try to make everything perfect. This delays releases and prevents you from:
- Getting real user feedback
- Generating revenue
- Learning what actually matters
- Building momentum

---

## The Solution: Enforced Constraints

### 7-Day Rule
**From idea to deployed V1: MAX 7 days**

Day 1: Research + validate idea (talk to 3 potential users)
Day 2-3: Build core feature only
Day 4: Add basic auth + payment
Day 5: Deploy + test
Day 6: Fix critical bugs only
Day 7: Launch (post on Reddit, Twitter, send to first users)

If you're not deployed by day 7, you're overthinking it.

---

## V1 Feature Limit: 3 Features MAX

### Example: Form-to-Database Tool
**V1 INCLUDES:**
1. Receive form webhook
2. Store in database
3. Send email notification

**V2 CAN ADD:**
- Data validation
- Custom field mapping
- Integration with CRMs
- Analytics dashboard
- etc.

### How to Enforce This
Before coding, write down your 3 features. If you think of a 4th, add it to a "V2 Ideas" list and IGNORE IT.

---

## Use Existing Solutions (Don't Build From Scratch)

### Authentication
- **Use**: Supabase, Firebase, Clerk, Auth0
- **Don't**: Build custom JWT system, OAuth flows, password reset

### Payments
- **Use**: Stripe Checkout, PayPal, Lemon Squeezy
- **Don't**: Build custom subscription logic, payment processing

### Database
- **Use**: Supabase, Firebase, PlanetScale, Neon
- **Don't**: Set up your own Postgres server, write complex migrations

### Hosting
- **Use**: Vercel, Netlify, Railway, Render (one-click deploy)
- **Don't**: Configure nginx, set up SSL certificates, manage servers

### Email
- **Use**: Resend, SendGrid, plain text emails
- **Don't**: Build HTML email templates, custom SMTP setup

### Design
- **Use**: Tailwind UI, shadcn/ui, DaisyUI (copy/paste components)
- **Don't**: Design from scratch, pixel-perfect layouts, custom CSS

---

## The "Good Enough" Checklist

Before you ship V1, answer these questions:

1. **Does it solve the core problem?**
   - [ ] Yes → Ship it
   - [ ] No → Fix only this, then ship

2. **Can a user sign up and use it?**
   - [ ] Yes → Ship it
   - [ ] No → Add basic auth, then ship

3. **Can you get paid for it?**
   - [ ] Yes → Ship it
   - [ ] No → Add Stripe link or manual invoice option, then ship

4. **Is it accessible online?**
   - [ ] Yes → Ship it
   - [ ] No → Deploy to Vercel/Netlify, then ship

If you answered Yes to all 4, you MUST ship. No excuses.

---

## Perfectionism Red Flags

If you catch yourself saying/thinking these, STOP IMMEDIATELY:

- "I should add just one more feature..."
- "Let me refactor this code first..."
- "The design doesn't look professional enough..."
- "I need to add error handling for edge cases..."
- "What if someone tries to..."
- "I should write tests before shipping..."
- "Let me optimize this query..."
- "The mobile version needs work..."
- "I should add loading states..."
- "This needs better documentation..."

### The Counter-Response
"This is a V2 problem. Ship V1 first."

---

## What Actually Matters in V1

1. **Does it work?** (70% of the time is fine)
2. **Does it solve the problem?** (for the happy path)
3. **Can someone pay you?** (even manually)
4. **Is it online?** (even if ugly)

Everything else is V2.

---

## Permission to Ship Ugly Code

You have permission to ship:
- Inline styles
- Hardcoded values
- Ugly UI
- Basic error messages ("Something went wrong")
- Code with TODO comments
- No loading states
- Desktop-only designs
- Plain text emails
- Manual processes (you can automate later)

**Why?** Because shipped ugly code > perfect unshipped code

---

## The Reality Check

### Question: "What if users complain about X?"

**Answer**: If you have users complaining, you've WON. That means:
1. You shipped
2. People are using it
3. You're getting feedback
4. You can fix it in V2

Most projects never get to the "users complaining" stage because they never ship.

---

## Emergency Brake

If you've been working on a project for more than 7 days and haven't shipped, do this:

1. Stop coding immediately
2. List every feature you've built
3. Cross out everything except the core 3
4. Delete or comment out that code
5. Deploy what's left
6. Ship it TODAY

---

## Success Metrics for V1

**Good metrics:**
- Days to launch: < 7
- Number of features: ≤ 3
- First paying user: within 30 days of launch
- User feedback received: > 0

**Bad metrics:**
- Code quality
- Test coverage
- Design polish
- Performance benchmarks

You can measure those AFTER you have revenue.

---

## The Shipping Commitment

I commit to:
1. Ship V1 within 7 days of starting
2. Limit V1 to 3 core features
3. Use existing tools/templates/services
4. Ignore perfectionism red flags
5. Get user feedback before building V2

Signed: _________________ Date: _________________

---

## Claude Code's Role

When working with Claude Code on Side Hustle projects:

**Claude should:**
- Remind you of the 7-day limit
- Push back if you add features beyond the core 3
- Suggest using existing services instead of building custom
- Actively encourage shipping "good enough" code
- Call out perfectionism red flags

**You should tell Claude:**
- "Stop me if I'm over-engineering this"
- "Remind me of the shipping rules"
- "Is this a V1 or V2 feature?"

---

## Remember

**Your goal is not to build perfect software.**

**Your goal is to:**
1. Solve a real problem
2. Get it in front of users
3. Get feedback
4. Generate revenue
5. Iterate based on real data

Perfect is the enemy of shipped. SHIP IT.
