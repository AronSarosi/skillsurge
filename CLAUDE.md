# CLAUDE.md - SkillSurge Project Memory

## About Me
I'm Aron Sarosi. I moved from Budapest to London at 17, worked in management consulting, then transitioned into data science. I was a Data Science Team Lead at Legal & General. During the pandemic, I learned coding through Le Wagon bootcamp and built a Python course on Udemy that became the platform's highest rated Python course (4.9/5 rating). I'm now a full-time course creator and entrepreneur building SkillSurge.

## About SkillSurge
SkillSurge is an online education platform with two tracks: Python and AI. The website is skillsurge.co, hosted on GitHub Pages from this repo. The domain DNS is managed through Squarespace.

### Current Products & Assets
- Python Masterclass on Udemy (4.9/5 - highest rated Python course)
- **AI Starter Guide** - free lead magnet, collected via ConvertKit AI form (captures email, delivers guide)
- **Plug & Play AI Setup** - $27 paid product (currently on waitlist via AI Tools Waitlist form)
- **SkillSurge Community** - waitlist, collected via ConvertKit community form
- Free Python resource: 8-Week Python Roadmap (via ConvertKit Python form)
- Email marketing through Kit (ConvertKit) with separate sequences for Python and AI subscribers
- Kit landing page: aronsarosi.kit.com/python-roadmap

### ConvertKit Form IDs
- Python Roadmap: `9068573`
- AI Starter Guide: `9110856`
- Community Waitlist: `9125775`
- AI Tools Waitlist (Plug & Play): `9125807`
- API Key: `U-0B6YZOem0yuvBzMaKDgQ`

### Business Strategy
- Phase 1 (now): Build audience through free resources, daily Facebook group posts, grow email list
- Phase 2 (parallel): Build a real SaaS product with AI tools, document the journey publicly
- Phase 3: Launch AI course/community on Skool ($49-97/month) teaching how to build with AI
- Phase 4: Cohort coaching (summer target)
- SkillSurge is the education brand. SaaS products are built separately but become content/proof for SkillSurge

### Email Strategy
- Python subscribers get Python email sequence promoting the Udemy course
- AI subscribers get AI email sequence (being built) promoting future AI course/community
- If someone has both tags, they get the AI sequence (higher priority track)
- Emails feel personal (from Aron), not corporate (from SkillSurge)
- Style: Sabri Suby conversational approach - short paragraphs, one thought per line, occasional dry humour

## Website Structure
```
skillsurge/
  index.html              -- Main landing page (skillsurge.co)
  business.html           -- B2B landing page (skillsurge.co/business) — font: Poppins
  python-projects/
    index.html            -- Interactive Python projects page (skillsurge.co/python-projects)
  blog/
    index.html            -- Blog listing page (skillsurge.co/blog)
    2026-python-roadmap/
      index.html          -- First blog post
    _template.html        -- Reusable template for future blog posts
  Aron Sarosi.png         -- Founder headshot (used in Meet the Founder section)
  CLAUDE.md               -- This file
  robots.txt              -- Crawl directives
  sitemap.xml             -- All URLs listed
```

### Homepage Section Order (index.html)
1. **Hero** (bg-a #1A1A2E) - "Master AI for free." headline, AI Starter Guide CTA
2. **AI Capabilities** (bg-b #171728) - 4-item accordion (see below)
3. **Our Offering** (bg-a) - Plug & Play AI Setup card + SkillSurge Community card
4. **Reviews** (bg-a) - Ticker rows with student quotes
5. **Learn Python** (bg-b) - Python Masterclass product card
6. **Meet the Founder** (bg-deep #13132A) - Aron bio + round headshot
7. **Footer**
8. **AI Tools Waitlist Modal** - ConvertKit form 9125807
9. **Onboarding Modal** - 3-step: name/email → AI or Python → success

### AI Capabilities Accordion (4 boxes, 2x2 grid)
Boxes go top-left → top-right → bottom-left → bottom-right (progression: entry to advanced):

| Position | Title | Description theme | Tools |
|----------|-------|-------------------|-------|
| Top-left | **AI Strategy Partners** | On-demand advisors: copy, visuals, plans, landing pages; Custom GPTs/Projects | Claude, ChatGPT, Gemini |
| Top-right | **Automated Workflows** | Connect AI to tools you use; pipelines that run without you | Make, n8n, Zapier |
| Bottom-left | **Custom AI Agents** | Build full products from a conversation: websites with Stripe, SaaS dashboards, e-commerce | Claude Code, Codex, Cursor |
| Bottom-right | **24/7 Autonomous Agents** | Runs on messaging apps while you sleep, no prompting needed | OpenClaw |

CSS: `.offering-item.open .offering-desc { max-height: 280px; }` — increase if descriptions get longer.
Tool tags: `.tool-tag` pills styled with subtle border, gray text, 12px font.

## Design Preferences & Brand Rules

### Colors
- Primary background: #1A1A2E (Dark Navy)
- Secondary background (alternate sections): #171728 (subtle, barely darker than navy — used for every other section)
- Secondary surface: #222240 (standalone pages like python-projects)
- Accent: #4CAF50 (Surge Green) - CTAs, highlights, ticks, "Surge" in wordmark
- Gold: #E5A839 - ratings, stars, premium accents
- Border: #2A2A50 - subtle borders and dividers
- Text on dark: #D0D0E8 (primary), #9999BB (secondary), #8888AA (tertiary/footer)
- White: #FFFFFF - headings on dark backgrounds

### Typography
- Web: Poppins (Google Fonts) - Bold for headings, Regular for body
- Code: Fira Code for code blocks
- Minimum body text size: 11pt in PDFs, 16-17px on web
- If text looks small, make it bigger. Always.

### Strict Rules - ALWAYS Follow These
1. **Green ticks for bullet points** - never use dots, dashes, or squares. Always green (#4CAF50) tick marks
2. **No em-dashes** - never use long em-dashes (they look AI-generated). Use short hyphens (-) only
3. **No arrows in buttons** - never put arrows, chevrons, or symbols inside CTA buttons. Text only
4. **Consistent backgrounds** - keep background color the same across a page. No darker patches for code blocks or text boxes
5. **No small text** - body text under 11pt in PDFs or 16px on web is too small
6. **Generous spacing** - when in doubt, add more whitespace. Cramped layouts always need fixing
7. **Brand name** - always "SkillSurge" with capital S's. Never "Skillsurge" or "skillsurge"
8. **Buttons** - green background, white bold text, rounded corners (10px), text like "Visit SkillSurge" not "skillsurge.co"
9. **Logo placement in PDFs** - cover page top-left only, final page bottom center, footer text on other pages
10. **No generic AI copy** - avoid "unlock your potential", "embark on a journey", "game-changer", "dive in"

### Code Block Styling (Website)
- VS Code Material theme syntax highlighting
- Keywords: #C792EA (purple)
- Built-ins: #82AAFF (blue)
- Strings: #C3E88D (green)
- Numbers: #FFCB6B (gold)
- Comments: #546E7A (gray italic)
- Default text: #EEFFFF (off-white)
- Copy-to-clipboard button on all code blocks

### Website Specifics
- Subtle dot grid background pattern on main site
- Green radial glow behind key sections for depth
- Cards: collapsible on python-projects page, one open at a time, hover shows green border
- Onboarding modal collects: name, email, interests (Python/AI/both)
- "Udemy's #1 highest rated Python course (4.9/5)" should always be a standalone prominent line, never buried in paragraphs
- Student review quotes from Yulia, Faaiz, and Zain are approved for use

## Working Preferences

### How I Like to Work
- I prefer direct, actionable output over theoretical explanations
- Show me the result first, explain later if I ask
- When I ask for changes, implement them fully even if it means rebuilding from scratch
- I'd rather wait longer for quality work than get something quick and mediocre
- Don't ask me lots of questions before starting - make smart decisions and I'll give feedback
- When making website changes: edit the files, commit, and push. Minimise back-and-forth

### Content Tone
- Conversational and direct, like a smart friend giving advice
- Short sentences. Short paragraphs. Especially in emails
- Confident but not arrogant
- British English spelling (colour, favourite, programme, analyse, etc.)
- Occasional dry humour in parenthetical asides
- Never corporate or formal

### What Annoys Me
- Text that's too small (I've asked for bigger text multiple times)
- Darker background patches inside content areas (keep backgrounds uniform)
- Long em-dashes anywhere
- Arrows inside buttons
- Having to iterate many times on something that should have been right the first time
- Pay-per-use pricing models
- Generic AI-sounding copy

## Key URLs
- Website: https://skillsurge.co
- Python Projects: https://skillsurge.co/python-projects
- Kit Landing Page: https://aronsarosi.kit.com/python-roadmap
- Udemy Course: https://udemy.com/course/python-masterclass-complete-python-bootcamp-for-beginners
- GitHub: https://github.com/AronSarosi/skillsurge

## Proof Points to Use
- "Udemy's #1 highest rated Python course (4.9/5)" - use prominently everywhere
- 10+ years as a data scientist
- Former Data Science Team Lead at Legal & General
- Le Wagon bootcamp graduate
- Building SkillSurge entirely with AI tools (this IS the proof of concept)
