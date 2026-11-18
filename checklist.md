# Griha Architects — Client Placeholder Hand-Off Checklist

This checklist summarizes all placeholder items in the Griha Architects website codebase that require client confirmation or final asset replacement before production deployment.

---

### 1. Domain Configuration
- **Placeholder in Code:** `https://[DOMAIN]`
- **Locations Used:**
  - `sitemap.xml` (all URL entries)
  - `robots.txt` (Sitemap URL)
  - Canonical link tags `<link rel="canonical" href="...">` across all HTML pages
  - Open Graph (`og:url`, `og:image`) and Twitter card meta tags
  - Schema.org JSON-LD structured data (`@id`, `url`, `logo`, `image`)
- **Action Required:** When the client registers their domain (e.g., `https://grihaarchitects.com`), perform a search-and-replace for `https://[DOMAIN]` across all files with the live production URL.

---

### 2. Photography & Portfolio Imagery
- **Placeholders in Code:**
  - `assets/images/project-elevation.svg`
  - `assets/images/project-kitchen.svg`
  - `assets/images/project-office.svg`
  - `assets/images/project-clinic.svg`
  - `assets/images/project-floorplan.svg`
  - `assets/images/project-institution.svg`
- **Badge in Code:** `[PROJECT PHOTO PENDING CLIENT UPLOAD]`
- **Action Required:** Provide high-resolution, compressed WebP/JPG photographs of real completed or under-construction projects in Prayagraj. Replace placeholder files in `assets/images/` and update `alt` text if specific project names/details change.

---

### 3. Founder Portrait & Council of Architecture (COA) Credentials
- **Placeholder in Code:** `assets/images/founder-placeholder.svg`
- **Badges in Code:**
  - `[FOUNDER PHOTO PENDING CLIENT UPLOAD]`
  - `[COA REGISTRATION & CREDENTIAL CONFIRMATION PENDING CLIENT SUBMISSION]`
- **Action Required:**
  - Provide a high-resolution professional portrait of Ar. Chandan Singh (Chandan Singh Bhartiya) in 4:5 aspect ratio (e.g., 800×1000 px).
  - Provide Council of Architecture (COA) registration number (e.g., `CA/YYYY/XXXXX`) and educational background for inclusion in `about.html` and JSON-LD schema.

---

### 4. Google Maps Embed URL & Google Business Profile CID
- **Placeholder in Code:** `[GOOGLE MAPS EMBED URL PENDING VERIFIED CLIENT GOOGLE BUSINESS PROFILE CID]`
- **Location Used:** `contact.html` (Google Map iframe container)
- **Current Embed:** Coordinates query centered on Vinayak Triveni Tower, Kanpur–Allahabad Highway, Civil Lines, Prayagraj 211001.
- **Action Required:** Provide the official Google Maps Embed URL generated directly from the verified "Griha Architects" Google Business Profile in Civil Lines.

---

### 5. Verified Client Reviews & Ratings
- **Badge in Code:** `[REVIEW PENDING CLIENT CONFIRMATION]`
- **Rule Followed:** Per SEO guidelines, **no fake reviews, ratings, or star counts were invented**, and `aggregateRating` schema has been omitted.
- **Action Required:** When genuine Google reviews or signed client endorsements are gathered:
  1. Add verified testimonial quotes and client names to `index.html` and `about.html`.
  2. Optionally add `Review` or `aggregateRating` JSON-LD schema once at least 3–5 verified public reviews exist.

---

### 6. Pricing & Quotation Guidance
- **Badge in Code:** `[PRICE PENDING]` / `[PRICE PENDING SITE SURVEY & SCOPE CONFIRMATION]`
- **Rule Followed:** No hypothetical prices or per-square-foot rates were invented.
- **Action Required:** If Griha Architects wishes to publish starting consult fees (e.g., initial 2D map drafting fee or per-sq-ft construction rate), replace these placeholders in `services.html` and `projects.html`.

---

### 7. Social & Authority Profiles (`sameAs`)
- **Placeholder in Code:** `"sameAs": []` in JSON-LD on `index.html` and `about.html`
- **Action Required:** Insert live URLs for:
  - Official LinkedIn profile / company page
  - Instagram profile (architecture portfolio)
  - Facebook page
  - Council of Architecture directory listing
  - Justdial / IndiaMART verified business listing (if maintained)

---

### Summary Checklist Table

| Item | Current State | Required Client Asset | Affected Files |
| :--- | :--- | :--- | :--- |
| **Domain** | `https://[DOMAIN]` | Final Registered Domain | All HTML, CSS, `robots.txt`, `sitemap.xml` |
| **Project Photos** | SVG wireframe schematics | 6+ High-res WebP/JPG photos | `assets/images/`, `projects.html`, project details |
| **Founder Photo** | SVG silhouette badge | Professional portrait photo | `assets/images/founder-placeholder.svg`, `about.html` |
| **COA Credentials** | Marked placeholder | COA Registration Number | `about.html`, JSON-LD schema |
| **Google Map** | Query fallback iframe | Official Google Business embed code | `contact.html` |
| **Client Reviews** | Marked placeholder badge | 3–5 Authentic client testimonials | `index.html`, `about.html` |
| **Pricing / BOQ** | Marked placeholder badge | Rate cards or consult terms | `services.html`, `projects.html` |
| **Social / sameAs** | Empty array `[]` | Social media & directory profile links | `index.html`, `about.html` (JSON-LD) |
