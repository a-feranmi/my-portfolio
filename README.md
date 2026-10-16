# Feranmi Amole · Portfolio

**Live site:** [theferanmiamole.netlify.app](https://theferanmiamole.netlify.app)

The personal portfolio of **Oluwaferanmi (Feranmi) Amole**, a Data Analyst, BI Developer and Analytics Engineer based in Lagos, Nigeria, working with teams across time zones.

I build the dashboards teams make decisions from, and the data layers underneath them: semantic models, warehouse tables and tested pipelines. This site brings that work together in one place: who I am, what I've built, and how to work with me.

---

## What's on the site

| Page | What you'll find |
|---|---|
| **Home** | An interactive globe that shows how my working day overlaps with yours (search any city in the world), a blueprint/build slider for five featured projects, and live client feedback |
| **About** | My story, work experience, a "CV as a dashboard" report, the tools I use and what I use each one for, and how I deliver a project |
| **Projects** | Every project with the problem, the data, what I built and what it found, including results that didn't go to plan |
| **FAQ** | Answers for recruiters, hiring managers and clients, searchable by topic |
| **Contact** | Email, LinkedIn, GitHub and WhatsApp, plus a message form |
| **Hire me** | An interactive SQL console where you can query a small "database about me" |

## Featured work

- **E-Commerce Retail Sales Analysis:** a 3-page Power BI report (ZoomCharts challenge) that found loyal customers drive 84.6% of revenue
- **BredgePulse:** an ML web app that flags at-risk client engagements early
- **MedShare:** an MSc capstone platform for inter-pharmacy drug redistribution in Lagos
- **Global B2B Sales Report:** a 9-table Power BI star schema with what-if analysis
- **HR Attrition Dashboard:** corrected an attrition rate from about 50% to the true 33.4%

## Toolkit

**BI & reporting:** Power BI · DAX · Power Query · Tableau · Looker · Data Studio · Excel
**Data & warehouse:** SQL · BigQuery · Snowflake · PostgreSQL · dbt
**Code:** Python
**Learning now:** Airflow · Spark

## How the site is built

A single, dependency-free static site, with no framework and no build step:

- **HTML, CSS and vanilla JavaScript** in one `index.html`, with hash routing between pages
- **Canvas and SVG** for the interactive pieces (the globe, the project blueprints, the CV dashboard)
- **`cities.json`**, a compact world-cities dataset (about 9,000 places with time zones), loaded only when someone searches the globe
- **Netlify Forms** for the contact form
- **Google Sheets** (published CSV) for client testimonials, shown only after I approve them
- Light and dark themes, responsive down to phone width, and reduced-motion support

```
├── index.html    the whole site
├── cities.json   world cities + time zones for the globe search
└── img/          project screenshots
```

Hosted on **Netlify**, deployed automatically from this repository on every push.

## Get in touch

- **Email:** [ample.oluwaferanmi26@gmail.com](mailto:ample.oluwaferanmi26@gmail.com)
- **LinkedIn:** [linkedin.com/in/oluwaferanmi-amole](https://www.linkedin.com/in/oluwaferanmi-amole/)
- **GitHub:** [github.com/a-feranmi](https://github.com/a-feranmi)
- **WhatsApp / call:** [+234 814 127 0590](https://wa.me/2348141270590)

Open to remote, hybrid and relocation roles, with 2 weeks' notice.

---

© Oluwaferanmi Amole. The design and content of this site are my own; please don't reuse them without permission.