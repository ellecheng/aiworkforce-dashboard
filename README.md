# aiworkforce-dashboard
A diagnostic tool for companies to compare against country average (India or Singapore depending on their matured/growth market) on 6 dimensions, which would provide recommendations on leadership behaviour and COE ownership to inform localisation strategy.  The AI readiness framework is developed through synthesizing 2 global workforce surveys: PwC's Global Workforce Hopes & Fears Survey and BCG's AI at Work series (APAC 2025 + Global 2026). This provides one view on AI adoption, trust towards leaders and culture transformation with customisable suggestion to companies in APAC, as a starting point.
surveys into six cross-report tensions, a leadership behaviour map, Singapore vs India localization, and a live org diagnostic tool — an AI-literacy capstone exploring AI adoption, trust, and culture transformation in APAC.

**[View the live dashboard →](https://ellecheng.github.io/aiworkforce-dashboard/)**

---
 
## Why I built this
 
I am interested in the intersection of AI adoption and culture/inclusion work. In large scale culture transformation work, insights from employee data are crucial to identify local nuance than one size fit all strategy. I wanted to have a hands-on capstone - using AI to research and synthesise reports on this topic, as well as visualise data in a digestible format. I was dependent on a business analyst which on average takes 2-3 working days to generate a dashboard, thus embarking on this project helped me understand the limitation and the benefits from using AI as a use case for HR.
 
## What it does
 
- **Org Diagnostic** — six sliders let you score your own organisation across
  the six tensions below (leadership support, trust, strategy clarity, training
  access, job security reassurance, and psychological safety). Toggle between
  two market benchmarks — a mature market (Singapore) and a hyper-growth market
  (India) — and each dial's progress ring shows your org's gap against that
  market's own average, flagged at 10 percentage points or more. A faint
  reference tick also shows where BCG's "high-performing" (Reshape/Invent)
  organisations sit, for context.
- **Tension drill-downs** — clicking any dial opens the tension behind it, in
  sequence T1 through T6: a bolded one-line conclusion, an italic supporting
  insight, and two source cards (PwC and BCG) that expand individually to show
  the specific statistics behind the claim, without disrupting the rest of
  the page.
- **COE Activation Map** — maps each of the six tensions to a concrete
  leadership behaviour and the HR Centre of Excellence best placed to own it
  (Inclusion, Talent Development, OD & Culture, Internal Comms, Total Rewards/ER).
  Click any COE chip to isolate the rows it owns.
  
## How it was built
 
I used Claude as a thinking and build partner across the full workflow:
extracting and cross-referencing findings from four source documents (two PwC
reports, two BCG decks), identifying where the two independently-fielded
surveys converged on the same six themes, translating those themes into a
leadership-behaviour and COE-ownership framework, and building the interactive
front end (vanilla HTML/CSS/JS, no frameworks, hosted on GitHub Pages). The
structure went through several iterations — starting as a linear scroll, then
rebuilt around the diagnostic as the entry point once it became clear that
was the more useful "living" artifact.
 
## A note on the data
 
All statistics are attributed to their source report and flagged where a
figure was read visually from a chart rather than stated in body text. The
diagnostic tool's benchmark scores are mapped onto a common 0–100 scale by
theme for comparability, since the two surveys ask different questions — and
that mapping, the 10-point gap threshold, and the leadership-behaviour and
COE recommendations are an editorial framework I built for this exercise, not
a finding from either report. The "job security reassurance" dimension in
particular is a derived proxy (built from optimism and job-loss-fear figures
in both reports) rather than a single directly-stated metric. Treat the
diagnostic as a starting structure for a real internal pulse survey, not a
substitute for one.
 
**Sources:**
- PwC, [Global Workforce Hopes and Fears Survey 2025](https://www.pwc.com/gx/en/issues/workforce/hopes-and-fears.html) — Global and [Singapore](https://www.pwc.com/sg/en/publications/hopes-and-fears.html) editions
- BCG, *AI at Work: Is Asia Pacific Leading the Way?* (APAC edition, October 2025)
- BCG, *AI at Work: Strategy Matters More Than Tools* (Global, Fourth Edition, June 2026)
## Built with
 
HTML / CSS / JavaScript, no build step — designed to be portable and
GitHub Pages-ready. Anthropic's Claude was used throughout for data synthesis,
framework design, and front-end development.
 
---
 
Elle Cheng · Values & Culture Transformation · Human-centric leadership in an AI era workforce
