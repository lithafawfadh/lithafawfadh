# GitHub Profile README Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Transform Mohamed Lithaf Awfadh's GitHub profile README into a minimal, extraordinary, Linear-inspired dark-mode showcase emphasizing real-world production engineering over academic clichés.

**Architecture:** Create an in-repo bespoke SVG header asset (`assets/header.svg`), replace rainbow shields and broken third-party stats with a high-impact metrics strip, curate a monochromatic `#161b22` tech stack, and structure an architectural project matrix with quantifiable client impacts.

**Tech Stack:** GitHub Flavored Markdown, SVG, Shields.io (monochromatic flat-square), Git.

---

### Task 1: Create the Bespoke Minimalist SVG Header Banner

**Files:**
- Create: `lithafawfadh/assets/header.svg`

- [ ] **Step 1: Create the `assets` directory and author `header.svg`**

Create `lithafawfadh/assets/header.svg` with a dark canvas (`#0d1117`), refined typography, subtle tech accent lines, and an availability badge:

```xml
<svg width="840" height="200" viewBox="0 0 840 200" fill="none" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Background Gradient -->
    <linearGradient id="bgGradient" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0d1117" />
      <stop offset="50%" stop-color="#161b22" />
      <stop offset="100%" stop-color="#0d1117" />
    </linearGradient>

    <!-- Accent Gradient Line -->
    <linearGradient id="accentGlow" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#30363d" stop-opacity="0" />
      <stop offset="25%" stop-color="#58a6ff" stop-opacity="0.8" />
      <stop offset="50%" stop-color="#7ee787" stop-opacity="0.8" />
      <stop offset="75%" stop-color="#58a6ff" stop-opacity="0.8" />
      <stop offset="100%" stop-color="#30363d" stop-opacity="0" />
    </linearGradient>

    <!-- Subtle Grid Pattern -->
    <pattern id="grid" width="24" height="24" patternUnits="userSpaceOnUse">
      <path d="M 24 0 L 0 0 0 24" fill="none" stroke="#21262d" stroke-width="0.75" stroke-opacity="0.6"/>
    </pattern>

    <!-- Drop Shadow for Tag -->
    <filter id="badgeShadow" x="-10%" y="-10%" width="120%" height="120%">
      <feDropShadow dx="0" dy="2" stdDeviation="3" flood-color="#000000" flood-opacity="0.5"/>
    </filter>
  </defs>

  <!-- Background Base -->
  <rect width="840" height="200" rx="10" fill="url(#bgGradient)" stroke="#30363d" stroke-width="1.2"/>
  <rect width="840" height="200" rx="10" fill="url(#grid)"/>

  <!-- Top Decorative Accent Line -->
  <rect x="40" y="1" width="760" height="2" fill="url(#accentGlow)" rx="1"/>

  <!-- Status Badge Container -->
  <g transform="translate(48, 36)">
    <rect width="210" height="24" rx="12" fill="#161b22" stroke="#30363d" stroke-width="1" filter="url(#badgeShadow)"/>
    <circle cx="14" cy="12" r="4" fill="#3fb950">
      <animate attributeName="opacity" values="1;0.4;1" dur="2.5s" repeatCount="indefinite"/>
    </circle>
    <text x="26" y="16" fill="#8b949e" font-family="-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif" font-size="11" font-weight="600" letter-spacing="1">AVAILABLE FOR INTERNSHIPS</text>
  </g>

  <!-- Name & Branding -->
  <text x="48" y="106" fill="#f0f6fc" font-family="-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif" font-size="32" font-weight="800" letter-spacing="1.5">MOHAMED LITHAF AWFADH</text>

  <!-- Engineering Discipline / Subtitle -->
  <text x="48" y="136" fill="#7ee787" font-family="-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif" font-size="13" font-weight="700" letter-spacing="2">SOFTWARE ENGINEER</text>
  <text x="228" y="136" fill="#8b949e" font-family="-apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif" font-size="13" font-weight="400" letter-spacing="1.2">·  FULL-STACK &amp; ENTERPRISE SYSTEMS</text>

  <!-- Subtle Architecture Philosophy Pill -->
  <g transform="translate(48, 154)">
    <text x="0" y="14" fill="#6e7681" font-family="ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace" font-size="11">building resilient distributed architectures &amp; production software</text>
  </g>

  <!-- Corner Minimalist Geometric Element -->
  <g transform="translate(730, 80)" stroke="#30363d" stroke-width="1.2" opacity="0.7">
    <circle cx="40" cy="40" r="28" fill="none" stroke-dasharray="4 4"/>
    <circle cx="40" cy="40" r="16" fill="none"/>
    <circle cx="40" cy="40" r="4" fill="#58a6ff"/>
  </g>
</svg>
```

- [ ] **Step 2: Validate SVG syntax**

Run:
```powershell
[xml](Get-Content "lithafawfadh\assets\header.svg") | Out-Null; Write-Host "SVG Valid"
```
Expected output: `SVG Valid`

- [ ] **Step 3: Commit the SVG asset**

```bash
cd lithafawfadh
git add assets/header.svg
git commit -m "feat: add bespoke minimalist SVG header banner"
```

---

### Task 2: Rewrite `README.md` with Minimalist & Extraordinary Content

**Files:**
- Modify: `lithafawfadh/README.md`

- [ ] **Step 1: Draft and write the new `README.md` content**

Replace `lithafawfadh/README.md` completely with:

```markdown
<div align="center">

  <img src="./assets/header.svg" alt="Mohamed Lithaf Awfadh - Software Engineer" width="100%" />

  <br/><br/>

  <!-- Monochromatic Quick Actions -->
  <a href="https://linkedin.com/in/lithafawfadh">
    <img src="https://img.shields.io/badge/LinkedIn-161b22?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:lithafawfadh@gmail.com">
    <img src="https://img.shields.io/badge/Email-161b22?style=flat-square&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://linkedin.com/in/lithafawfadh">
    <img src="https://img.shields.io/badge/Resume%20%2F%20CV-161b22?style=flat-square&logo=read-the-docs&logoColor=white" alt="Resume / CV" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Colombo%2C%20Sri%20Lanka-161b22?style=flat-square&logo=google-maps&logoColor=white" alt="Location" />
  </a>

</div>

<br/>

### ⚡ Proof of Work

| 04 | Active Users | Spring Boot 3 | Full-Stack |
| :---: | :---: | :---: | :---: |
| **Production Apps** | **Client-Commissioned** | **Enterprise Backend** | **React & TypeScript** |

---

### 👨‍💻 Engineering Profile

3rd-year Software Engineering undergraduate at **SLIIT** (Sri Lanka Institute of Information Technology), focused on architecting resilient enterprise backend services and modern data-intensive web applications.

Experienced across the full development lifecycle—from relational schema design and complex SQL migrations to secure **RESTful/JWT API design** and reactive **React/TypeScript** frontends. Proven track record taking client-commissioned solutions from initial system requirements to production deployments with active users.

---

### 🛠️ Technical Arsenal

<table>
  <tr>
    <td width="160"><b>Languages</b></td>
    <td>
      <img src="https://img.shields.io/badge/Java-161b22?style=flat-square&logo=openjdk&logoColor=white" alt="Java" />
      <img src="https://img.shields.io/badge/TypeScript-161b22?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
      <img src="https://img.shields.io/badge/JavaScript-161b22?style=flat-square&logo=javascript&logoColor=white" alt="JavaScript" />
      <img src="https://img.shields.io/badge/Python-161b22?style=flat-square&logo=python&logoColor=white" alt="Python" />
      <img src="https://img.shields.io/badge/SQL-161b22?style=flat-square&logo=postgresql&logoColor=white" alt="SQL" />
      <img src="https://img.shields.io/badge/C%2B%2B-161b22?style=flat-square&logo=c%2B%2B&logoColor=white" alt="C++" />
    </td>
  </tr>
  <tr>
    <td><b>Backend &amp; APIs</b></td>
    <td>
      <img src="https://img.shields.io/badge/Spring_Boot_3-161b22?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot" />
      <img src="https://img.shields.io/badge/Spring_Security-161b22?style=flat-square&logo=springsecurity&logoColor=white" alt="Spring Security" />
      <img src="https://img.shields.io/badge/Spring_Data_JPA-161b22?style=flat-square&logo=spring&logoColor=white" alt="Spring Data JPA" />
      <img src="https://img.shields.io/badge/Node.js-161b22?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js" />
      <img src="https://img.shields.io/badge/RESTful_APIs-161b22?style=flat-square&logo=postman&logoColor=white" alt="REST APIs" />
      <img src="https://img.shields.io/badge/JWT_Auth-161b22?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT" />
    </td>
  </tr>
  <tr>
    <td><b>Frontend</b></td>
    <td>
      <img src="https://img.shields.io/badge/React_18-161b22?style=flat-square&logo=react&logoColor=white" alt="React" />
      <img src="https://img.shields.io/badge/Tailwind_CSS-161b22?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
      <img src="https://img.shields.io/badge/Vite-161b22?style=flat-square&logo=vite&logoColor=white" alt="Vite" />
      <img src="https://img.shields.io/badge/React_Router-161b22?style=flat-square&logo=reactrouter&logoColor=white" alt="React Router" />
      <img src="https://img.shields.io/badge/Framer_Motion-161b22?style=flat-square&logo=framer&logoColor=white" alt="Framer Motion" />
    </td>
  </tr>
  <tr>
    <td><b>Database &amp; Cloud</b></td>
    <td>
      <img src="https://img.shields.io/badge/PostgreSQL-161b22?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
      <img src="https://img.shields.io/badge/Supabase-161b22?style=flat-square&logo=supabase&logoColor=white" alt="Supabase" />
      <img src="https://img.shields.io/badge/MySQL-161b22?style=flat-square&logo=mysql&logoColor=white" alt="MySQL" />
      <img src="https://img.shields.io/badge/Microsoft_Azure-161b22?style=flat-square&logo=microsoftazure&logoColor=white" alt="Azure" />
    </td>
  </tr>
  <tr>
    <td><b>Tooling &amp; Practice</b></td>
    <td>
      <img src="https://img.shields.io/badge/Git-161b22?style=flat-square&logo=git&logoColor=white" alt="Git" />
      <img src="https://img.shields.io/badge/GitHub-161b22?style=flat-square&logo=github&logoColor=white" alt="GitHub" />
      <img src="https://img.shields.io/badge/Postman-161b22?style=flat-square&logo=postman&logoColor=white" alt="Postman" />
      <img src="https://img.shields.io/badge/Linux-161b22?style=flat-square&logo=linux&logoColor=white" alt="Linux" />
      <img src="https://img.shields.io/badge/Agile%20%2F%20Scrum-161b22?style=flat-square&logo=jira&logoColor=white" alt="Agile" />
    </td>
  </tr>
</table>

---

### 🏛️ Featured Engineering Systems

| System | Architecture | Engineering Highlights | Source |
| :--- | :--- | :--- | :---: |
| **[FORT](https://github.com/lithafawfadh/FORT)** | React · TypeScript · Supabase · PostgreSQL · Tailwind | Real-time financial ledger & group fund management system built for 9 active users. Engineered with cascading SQL migrations, role-based row-level security (RLS), and live state sync. | [Code ↗](https://github.com/lithafawfadh/FORT) |
| **[Skill Connect](https://github.com/lithafawfadh/Skill-Connect)** | Spring Boot 3 · React 18 · Spring Security · MySQL | Full-stack skilled labor & equipment booking platform. Features 4 distinct role-based management dashboards, JWT stateless authentication, threaded messaging, and automatic late-fee engines. | [Code ↗](https://github.com/lithafawfadh/Skill-Connect) |
| **[Health Plus](https://github.com/lithafawfadh/Health-Plus)** | React · Azure · Appwrite · Tailwind | Cloud-enabled pharmacy management system deployed to Azure. Implements serverless backend functions, digital prescription tracking, and cashier/pharmacist access isolation. | [Code ↗](https://github.com/lithafawfadh/Health-Plus) |
| **[Sales Receipt Engine](https://github.com/lithafawfadh/Sales-Receipt-Generator)** | React · TypeScript · Tailwind CSS · Supabase | Mobile-first production receipt generator featuring high-throughput client bulk entries, dynamic tax/discount computation engine, and automatic PDF export. | [Code ↗](https://github.com/lithafawfadh/Sales-Receipt-Generator) |

---

<div align="center">
  <sub>Open to Software Engineering Internships (Dec 2026 / 2027) · On-site, Hybrid & Remote Worldwide</sub>
</div>
```

- [ ] **Step 2: Verify `README.md` formatting**

Run:
```powershell
Get-Item "lithafawfadh\README.md" | Select-Object Name, Length, LastWriteTime
```
Expected output: Non-empty file with recent write timestamp.

- [ ] **Step 3: Commit the updated `README.md`**

```bash
cd lithafawfadh
git add README.md
git commit -m "feat: redesign profile README with modern monochromatic aesthetic"
```

---

### Task 3: Visual & Content Verification

**Files:**
- Read: `lithafawfadh/README.md`
- Inspect: `lithafawfadh/assets/header.svg`

- [ ] **Step 1: Check all links and asset paths**

Verify that:
1. `./assets/header.svg` path matches the physical file.
2. All repository links (`FORT`, `Skill-Connect`, `Health-Plus`, `Sales-Receipt-Generator`) are correctly formatted.
3. No mention of "Dean's list" remains.
4. No third-party flaky stat widgets are present.

- [ ] **Step 2: Commit any final polish and verify git status**

```bash
cd lithafawfadh
git status
```
Expected output: `working tree clean`
