# Off My Desk Professionals — Website Project

## Overview

Landing page website for **Off My Desk Professionals (OMD)**, designed for Netlify deployment. Built as a premium, founder-led strategic partner site for Deb Shimojima — repositioned away from VA/staffing agency framing and toward a high-trust, creative + operations + AI consulting brand.

**Live Site:** https://www.offmydesk.pro  
**Contact:** Deb@offmydesk.pro  
**Founded:** Los Angeles, CA

---

## Last Updated

**April 12, 2026** — Visual polish pass: fixed header/logo display, corrected hero image cropping and alignment, removed broken `onerror` fallbacks from both nav and footer logos, tightened section spacing, added `privacy.html` and `terms.html` to resolve footer 404 errors. Zero console errors.

---

## Files

| File | Purpose |
|---|---|
| `index.html` | Full landing page — all sections |
| `blog.html` | Blog / Resources page with category filtering |
| `thank-you.html` | Post-form submission confirmation page |
| `privacy.html` | Privacy Policy page |
| `terms.html` | Terms of Use page |
| `netlify.toml` | Netlify build config, headers, redirects, caching |
| `robots.txt` | AI bot permissions (GPTBot, PerplexityBot, ClaudeBot, etc.) |
| `sitemap.xml` | XML sitemap for Google/AI search indexing |
| `llms.txt` | LLM guide for AI search citation accuracy (GEO) |
| `README.md` | This file |

### Blog Posts (blog/)
| File | Topic |
|---|---|
| `blog/custom-ai-gpt-small-business.html` | What a Custom AI GPT Actually Does |
| `blog/google-drive-organization.html` | The Google Drive Chaos Fix |
| `blog/linkedin-strategy-service-businesses.html` | LinkedIn ROI for Service Businesses |
| `blog/systems-not-tasks.html` | You Don't Have a Task Problem |
| `blog/sop-guide.html` | What Is an SOP and Why You Need One |
| `blog/ai-layoffs-launch.html` | Using AI to Launch After a Layoff |
| `blog/email-newsletter.html` | The 5-Part Email Newsletter That Gets Read |
| `blog/ai-small-business-gap.html` | 93% Say AI Helps. Only 14% Use It Fully. |
| `blog/website-as-sales-tool.html` | Your Website Is Your Best Sales Tool |
| `blog/inbox-management.html` | Inbox Zero Is Not the Goal |

---

## Sections in index.html

1. **Fixed Navigation** — sticky, mobile-responsive with hamburger
2. **Hero** — founder-led, with trust badges and dual CTAs
3. **Marquee Strip** — animated lime-colored service scroll
4. **Three Pillars** — Creative, Operations, Custom AI (Signature)
5. **About Deb** — founder story, values, pull quote, 20+ years badge
6. **Services** — full 4-pillar grid with detailed service lists
7. **Work With Me** — 4 packages with pricing, engagement models, "not sure" CTA
8. **First 30 Days** — 4-step onboarding roadmap
9. **Payment** — 4 payment method cards (Card, Bank, Invoice, PayPal)
10. **Booking** — Calendly + send message options
11. **Testimonials** — 6 real client quotes + industry served strip
12. **FAQ** — 16 accordion questions researched from 2026 trends
13. **Contact Form** — Netlify-powered, sends to Deb@offmydesk.pro
14. **Final CTA** — lime button booking close
15. **Footer** — logo, social links, navigation, email

---

## Package Names and Pricing

| Package | Position | Starting From |
|---|---|---|
| Essential | Solo founders, basic recurring support | $250/month |
| Growth | Growing businesses, content + ops | $750/month |
| Momentum | Scaling with AI-assisted systems | $1,500/month |
| AI Elite Build | Custom AI GPT development | $2,000+ per project |

**Decision note:** Package names were upgraded from Foundation/Pro/Premium/Elite to Essential/Growth/Momentum/AI Elite Build — more descriptive, less generic, and signals a value progression that aligns with the premium consultant positioning. The "from" pricing structure gives you room to add value and scope upward.

---

## Tone and Positioning

Work With Me section is styled **consultant-premium** — approachable in language, confident in pricing signals, structured for clarity. This is the right register for a 20+ year expert moving away from commodity VA framing.

---

## SEO and GEO Optimization

### Traditional SEO
- Canonical URL, meta title, meta description
- Semantic HTML5 (`<main>`, `<article>`, `<section>`, `<blockquote>`, `<cite>`)
- Proper heading hierarchy (one H1, H2s per section, H3s for subsections)
- Descriptive alt text on all images (keyword-rich, location-aware)
- `sitemap.xml` for Googlebot
- Responsive, mobile-first design (core ranking factor)

### GEO (Generative Engine Optimization / AI Search)
- `llms.txt` — guides ChatGPT, Claude, Perplexity, Gemini crawlers accurately
- `robots.txt` — explicitly allows GPTBot, PerplexityBot, ClaudeBot, anthropic-ai, Google-Extended
- `FAQPage` JSON-LD schema — FAQ content is cited heavily in AI Overviews and Perplexity
- `LocalBusiness` + `ProfessionalService` JSON-LD — entity-rich structured data
- GEO meta tags (`geo.region`, `geo.placename`, `geo.position`, `ICBM`)
- Open Graph + Twitter Card meta for social AI crawlers
- FAQ content researched from 2026 Reddit threads, Goldman Sachs surveys, LinkedIn research, and platform trend data

### AI Citation-Ready Content
The site uses clear, declarative language with specific service names, locations, pricing ranges, and expertise signals — the exact format AI search systems extract when building summaries.

---

## Contact Form Setup (Required After Deploy)

1. Deploy the site to Netlify via the Publish tab
2. In Netlify Dashboard: **Forms** > your site > **Form Notifications**
3. Add email notification: `Deb@offmydesk.pro`
4. Test the form once live

The form uses `data-netlify="true"` for zero-backend form processing.

---

## Calendly / Booking Links (Required Before Launch)

Search `https://calendly.com/deb-offmydesk` in `index.html` and `thank-you.html` and replace all instances with your actual Calendly URL (e.g., `https://calendly.com/yourname/discovery`).

---

## Images Required

Upload your photos to the `images/` folder before or after deploying:

| Filename | Description |
|---|---|
| `images/deb-hero.jpg` | Laptop/desk working photo — hero section |
| `images/deb-about.jpg` | Blazer standing photo — about section |
| `images/logo-dark.png` | Full logo — for dark (navy) backgrounds |
| `images/logo-icon.png` | Checkmark icon only — favicon |

All images are stored in the `images/` folder and load directly. The `onerror` fallbacks have been removed since the real photos are in place.

---

## Payment Processing

The site currently uses payment description cards (Credit Card via Stripe, Bank Transfer, Invoice, PayPal). To add live payment links:

1. Create a Stripe account and set up payment links for each package
2. Replace the `<a href="#contact">` links inside the `.pkg-cta` buttons with your Stripe payment link URLs
3. Optional: Add a Stripe Buy Button embed for a direct checkout experience

---

## To Add a Blog Post

Blog posts are currently static placeholder cards in `blog.html`. For a live blog with CMS-managed posts, consider:
- **Netlify CMS** (free, works with this setup)
- **Contentful** (free tier for small sites)
- Or simply add new `<article class="blog-card">` cards manually to `blog.html`

---

## Recommended Next Steps

1. ✅ Calendly link set to `https://calendly.com/deb-offmydesk` on all booking buttons
2. **Enable Netlify form notifications** — Dashboard → Forms → Form Notifications → `Deb@offmydesk.pro`
3. ✅ Photos uploaded to `images/` folder (hero, about, consulting, operations, logos)
4. **Add Stripe payment links** to package cards when Stripe account is ready
5. **Create Google Search Console** entry for https://www.offmydesk.pro and submit `sitemap.xml`
6. **Claim your Google Business Profile** with Los Angeles address for local SEO
7. ✅ 10 full blog posts live in `blog/` folder
8. **Activate Netlify CMS** — Dashboard → Identity → Enable → Git Gateway → Invite `Deb@offmydesk.pro` → Access at `/admin`
9. **Verify Open Graph preview** using https://opengraph.xyz before sharing socially

---

## Services on OMD vs Freelancing Platforms

**Your question:** Should core services (presentations, Google Drive, websites, LinkedIn) stay on OMD or only on platforms like Fiverr/Upwork?

**Recommendation:** Keep ALL core services on the OMD website. The platforms are a "bridge" — they should funnel toward direct client relationships, not be the destination. Presenting presentations, Google Drive organization, website builds, and LinkedIn strategy on the OMD site is important because:
- These are exactly what your clients search for when looking for someone like you
- They signal comprehensive capability and premium positioning
- They help Google and AI search systems understand your full service range
- They serve as proof that OMD delivers the full stack, not just one skill

The only adjustment is framing — on OMD, these are positioned as part of strategic retainer work or project-based engagements, not standalone $50 task orders.

---

&copy; 2026 Off My Desk Professionals — Los Angeles, CA
