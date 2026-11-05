# GitHub Profile README Design Specification
**Date:** 2026-11-05  
**Profile:** [lithafawfadh](https://github.com/lithafawfadh) (Mohamed Lithaf Awfadh)  
**Aesthetic:** Linear / Modern Tech Minimalist (Monochromatic Dark-Mode Harmonized)

---

## 1. Objectives & Design Principles
- **Minimal Yet Extraordinary:** Remove all visual noise, chaotic multi-colored badge tables, and third-party stat widgets that clutter the layout or fail to load.
- **Engineering-First Identity:** Position Lithaf as an active full-stack and systems engineer delivering real-world, client-commissioned software rather than a generic student portfolio.
- **Dark Mode Harmony:** Standardize on GitHub dark canvas (`#0d1117`) and slate accents (`#161b22`, `#30363d`), using monochromatic badges (`color=161b22`, white text and official logos).
- **Zero Academic Cliché:** Exclude "Dean's List" and resume-style coursework lists. Focus strictly on system design, deployed software, active users, and modern enterprise tech stack.

---

## 2. Profile Structure & Components

### Component 1: Minimalist SVG Header Banner
- **Format:** Bespoke, responsive SVG asset (`assets/header.svg`) hosted in the repository.
- **Dimensions:** 840x180 viewBox.
- **Palette:** `#0d1117` background with subtle `#30363d` 1px border and low-opacity geometric grid/mesh lines.
- **Typography:**
  - Name: `MOHAMED LITHAF AWFADH` (Inter/SF Pro style, tracking 2px, white `#f0f6fc`).
  - Role: `SOFTWARE ENGINEER · FULL-STACK & SYSTEMS ARCHITECTURE` (`#8b949e`, uppercase, tracking 1.5px).
  - Status Tag: `● AVAILABLE FOR INTERNSHIPS` (accent status indicator `#3fb950`).

### Component 2: Monochromatic Quick-Action Bar
- Clean horizontal badge strip styled in uniform `#161b22` slate:
  - `LinkedIn` (`style=flat-square&color=161b22&logo=linkedin&logoColor=white`) -> `https://linkedin.com/in/lithafawfadh`
  - `Email` (`style=flat-square&color=161b22&logo=gmail&logoColor=white`) -> `mailto:lithafawfadh@gmail.com`
  - `Resume / CV` (`style=flat-square&color=161b22&logo=read-the-docs&logoColor=white`) -> link to hosted CV/Resume
  - `Location: Colombo, Sri Lanka` (`style=flat-square&color=161b22&logo=google-maps&logoColor=white`)

### Component 3: Impact Strip ("By The Numbers")
- A clean markdown table or structured block replacing third-party stats:
  ```
  ┌───────────────────────┬───────────────────────┬───────────────────────┬───────────────────────┐
  │          04           │     Active Users      │     Spring Boot 3     │      Full-Stack       │
  │   Production Apps     │ Client-Commissioned   │ Enterprise Backend    │  React & TypeScript   │
  └───────────────────────┴───────────────────────┴───────────────────────┴───────────────────────┘
  ```

### Component 4: Executive Narrative
- High-density, professional two-paragraph overview:
  > 3rd-year Software Engineering undergraduate at **SLIIT**, focused on building scalable, reliable enterprise backends and modern web applications.
  >
  > Experienced in architecting end-to-end systems with **Spring Boot 3**, **Spring Security (JWT)**, **PostgreSQL/Supabase**, and **React/TypeScript**. Proven track record taking client-commissioned solutions from initial database schema design to production deployment with active users.

### Component 5: Monochromatic Tech Stack
Grouped with uniform dark badges (`style=flat-square&color=161b22&logoColor=white`):
- **Languages:** Java, TypeScript, JavaScript, Python, SQL, C++
- **Backend & APIs:** Spring Boot 3, Spring Security, Spring Data JPA, Node.js, RESTful APIs
- **Frontend:** React 18, TypeScript, Tailwind CSS, Vite, Framer Motion
- **Database & Cloud:** PostgreSQL, Supabase, MySQL, Microsoft Azure
- **Tools & Workflow:** Git, GitHub, Postman, Linux, Agile / Scrum

### Component 6: Architectural Project Showcase
A high-signal table highlighting production complexity, active user metrics, and code links:

| System | Architecture | Engineering Highlights | Source |
| :--- | :--- | :--- | :---: |
| **FORT** | React, TypeScript, Supabase (PostgreSQL), Tailwind | Multi-tenant financial ledger with cascading SQL migrations, role-based access, and real-time sync. Serving 9 active users. | [Code ↗](https://github.com/lithafawfadh/FORT) |
| **Skill Connect** | Spring Boot 3, React 18, Spring Security, MySQL | Service marketplace featuring 4 role-based dashboards, JWT authentication, and automated fee calculations. | [Code ↗](https://github.com/lithafawfadh/Skill-Connect) |
| **Health Plus** | React, Microsoft Azure, Appwrite | Cloud pharmacy workflow engine deployed to Azure with serverless functions and prescription tracking. | [Code ↗](https://github.com/lithafawfadh/Health-Plus) |
| **Sales Receipt Engine** | React, TypeScript, Tailwind CSS, Supabase | High-throughput receipt generator with automated client bulk calculation engine and invoice storage. | [Code ↗](https://github.com/lithafawfadh/Sales-Receipt-Generator) |

### Component 7: Minimal Footer & Availability
- Single-line discreet footer:
  `Available for Software Engineering Internships (Dec 2026 / 2027) · Open to On-site, Hybrid & Remote opportunities.`

---

## 3. Success Criteria
1. Fully responsive across desktop and mobile devices.
2. Zero broken images, third-party rate-limit issues, or clashing colors.
3. Clean rendering on GitHub's native dark and dim modes.
4. Professional tone reflecting a mature engineer.
