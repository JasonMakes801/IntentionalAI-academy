# IntentionalAI.academy Landing Page

## Project Overview

A landing page for a premium 1:1 AI coding setup service targeting non-technical executives and business professionals who feel left behind as their teams adopt AI tools.

**Core value proposition:** "Your team is already using AI coding tools. In one hour, I'll get you caught up."

**Target audience:** Directors, VPs, founders, product managers—people with budget authority who need hands-on AI capability, not theory.

**Emotional driver:** Fear of looking uninformed to their own teams. 94% of executives claim AI expertise but only 8% actually have it.

## Tech Stack

- **Framework:** Vue 3 via CDN (no build step, single HTML file)
- **Styling:** Tailwind CSS via CDN
- **Hosting:** Vercel (static deploy)
- **Booking:** Calendly embed (handles scheduling + Stripe payment)
- **Domain:** IntentionalAI.academy

## Design Direction

**Aesthetic:** Refined, confident minimalism. Think McKinsey or top-tier executive coaching—not startup playful, not developer techy.

**Typography:** 
- Headlines: A distinctive serif or refined sans-serif (Google Fonts: Playfair Display, Libre Baskerville, or DM Sans)
- Body: Clean, readable (Source Sans Pro, DM Sans)
- Avoid: Inter, Roboto, anything that screams "tech startup"

**Color palette:**
- Primary: Deep navy or charcoal (#1a1a2e or #0f172a)
- Accent: Warm gold or refined teal for CTAs
- Background: Off-white or subtle warm gray
- High contrast, confident, not trendy gradients

**Tone:** Direct, assured, no jargon. Speak to their anxiety without being condescending. Short sentences. No exclamation marks.

## Page Structure

### 1. Hero Section
- Headline addressing the fear directly
- Subheadline with the solution (1 hour, get caught up)
- Single CTA button to pricing/booking
- Optional: Jason's face (builds trust)

**Example copy:**
> "Your team is building with AI. You're not."
> 
> "In one focused hour, I'll get you set up with Claude Code and show you how to actually use it. No fluff, no theory—just the skills to keep up."

### 2. The Problem (Brief)
2-3 sentences max. Acknowledge what they're feeling.

> "Your direct reports are shipping features with AI tools you've never touched. You're nodding along in meetings, hoping no one asks for details. That ends today."

### 3. What You Get (Tiered Pricing)

Three tiers:

**STARTER — $175**
- 1-hour live screen-share session
- VS Code + Claude Code installed and configured
- Your first CLAUDE.md file written together
- Build something real with your own data
- Recording of the session

**PROFESSIONAL — $350**
- Everything in Starter
- 48-hour async support via WhatsApp/email (for when you get stuck)
- Second 1-hour follow-up session within 2 weeks
- Personalized "what to build next" roadmap

**EXECUTIVE — $750**
- Everything in Professional
- Pre-session: I review your business context and prepare custom examples
- Four follow-up sessions over 4 weeks
- Priority async support
- Monthly check-in call for 3 months

Display as clean cards, side by side on desktop, stacked on mobile.

### 4. About / Credibility
Brief bio establishing relevant experience:
- Integration Engineer supporting Disney, Netflix, Warner Brothers
- Built ML systems in production
- Self-taught coder who understands the non-technical perspective

Photo of Jason. First name only is fine.

### 5. How It Works
Simple 3-step:
1. Book your session and pay
2. Before we meet: send a spreadsheet or data file you work with
3. We build something real together in one hour

### 6. FAQ (Optional, can add later)
- "Do I need any coding experience?" → No
- "What if I use Windows?" → Works fine
- "What's Claude Code?" → Brief explanation

### 7. Final CTA
Repeat the booking button. Maybe with urgency: "Limited slots each week."

## Calendly Integration

Use Calendly's inline embed. The embed handles:
- Showing available time slots
- Collecting payment via Stripe
- Sending calendar invites

Create three separate Calendly event types, one per tier:
- Starter Setup ($175)
- Professional Setup ($350)  
- Executive Setup ($750)

Embed approach: Either three separate embeds in the pricing cards, or one primary embed with event type selection.

For now, use placeholder Calendly URL: `https://calendly.com/intentional-ai/setup`

## File Structure

```
/
├── index.html      # Single page with Vue + Tailwind via CDN
├── vercel.json     # Optional, for any routing config
└── README.md       # Deployment notes
```

## Vercel Deployment

1. Push to GitHub repo
2. Connect repo to Vercel
3. Auto-deploys on push
4. Add custom domain: IntentionalAI.academy

No build step needed—Vercel serves static HTML directly.

## Future Additions (Not Now)

- Email capture for "not ready yet" visitors
- Automated pre-session questionnaire (OS, goals, data file upload)
- Testimonials section (after first customers)
- Blog/content for SEO

## Development Notes

- Mobile-first responsive design
- Fast load time (no heavy assets)
- Accessible (proper contrast, semantic HTML)
- Test Calendly embed on mobile

## Voice & Copy Guidelines

- Never say "leverage" or "empower"
- Never use exclamation marks
- Short paragraphs, one idea each
- Address them as an equal who happens to need a specific skill
- Confident but not arrogant
- Acknowledge their intelligence—they're successful, just not at this one thing

## Example Competitor Reference

Look at executive coaching sites like BetterUp's individual pages, or high-end consulting—not Fiverr, not typical SaaS landing pages. The aesthetic should say "this costs money and it's worth it."
