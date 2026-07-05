   # ISO Security Dossier

An interactive, 3D "security clearance dossier" built for the RKRF MAY Internship task — a website covering ISO/IEC 27002:2022 clauses 5.16–5.20 (Identity Management, Authentication Information, Access Rights, Supplier Relationships, Supplier Agreements) plus the full ISO/IEC 27001 management system and control catalog.

**Live demo:** enable GitHub Pages (see below) and this line will point to it.

## What's inside

- **3D identity badge** in the hero — tilts in real 3D as you move your cursor, built with pure CSS `transform-style: preserve-3d`
- **Terminal boot sequence** — a typing animation that "loads" each control on page load
- **Control Deck** — clickable, tilting cards for clauses 5.16–5.20, each expanding into full requirements, audit evidence, and a real excerpt from the Tech Solutions / CloudSecure case study
- **PDCA Cycle explorer** — ISO 27001 clauses 4–10 grouped into Plan / Do / Check / Act, with expandable detail per clause
- **Full Control Catalog** — all 93 ISO/IEC 27002:2022 controls (Organizational, People, Physical, Technological), searchable and filterable
- **Case File** — a password-policy table and supplier compliance snapshot pulled from the reference documents

No build step, no dependencies — it's a single self-contained `index.html` (fonts load from Google Fonts CDN, everything else is inline CSS/JS).

## Running it locally

Just open `index.html` in any browser. Or, from this folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

**GitHub Pages**
1. Push this repo to GitHub (see below).
2. Go to **Settings → Pages** on the repo.
3. Under "Build and deployment", set Source to `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. Save — your site will be live at `https://<username>.github.io/<repo-name>/` within a minute or two.

**Vercel**
1. Import this repo at [vercel.com/new](https://vercel.com/new).
2. No framework preset needed — leave build settings blank (it's static HTML).
3. Deploy.

## Source material

Built from the ISO/IEC 27002:2022 and ISO/IEC 27001 reference PDFs assigned for the internship task, including the "Tech Solutions" access control, password management, and supplier agreement case studies.
