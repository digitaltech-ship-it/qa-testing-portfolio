# QA Testing Portfolio — Rosalyn Olivia Castro Lopez

Manual and API testing evidence from my own AI-powered web/PWA projects, done while studying the **ISTQB Foundation Level (CTFL)** syllabus through SSTQB/HASTQB.

📧 castrorosol78@gmail.com | 📍 Lima, Peru — Remote Worldwide | [Portfolio](https://pixelgoddessbo.pages.dev)

---

## 🧪 About this repository

This repo documents hands-on QA practice I'm doing on real projects I've built (PWAs, e-commerce, and business landing pages), applying ISTQB fundamentals to backend API testing, responsive UI testing, and bug reporting.

---

## 1. Backend / API Testing (CRUD)

**Tool used:** Thunder Client (VS Code)
**Project:** Sexto Continente backend / practice API

Tested Create, Read, Update, and Delete operations, validating status codes, response payloads, and error handling.

| Operation | Method | Result | Notes |
|---|---|---|---|
| Create | POST | `201 Created` | Verified response returned correct `id` and matched submitted body |
| Read | GET | `200 OK` | Verified payload structure (`userId`, `id`, `title`, `body`) |
| Read (invalid ID) | GET | `404 Not Found` | Confirmed API correctly rejects nonexistent resource |
| Update | PUT | `200 OK` | Verified updated fields returned correctly in response |
| Delete | DELETE | `200 OK` / `404 Not Found` | Tested both valid and invalid resource deletion |
| Malformed request | POST | `500 Internal Server Error` | Found that invalid JSON body causes an unhandled server error (`SyntaxError: Unexpected token`) |
| Invalid URL | GET / DELETE | `Error: Invalid URL` | Documented client-side validation gap when URL formatting is incorrect |

**Screenshots:** `/screenshots/api-testing/`
*(add your Thunder Client screenshots here — GET, POST, PUT, DELETE, and the error cases)*

**Key takeaway:** Practiced recognizing the difference between expected error responses (404) and unhandled server errors (500) — an important distinction in defect severity/priority classification.

---

## 2. Cross-Device / Responsive Testing

**Tool used:** Responsive Viewer
**Project:** Sexto Continente (exclusivesextocontinente.pages.dev)

Tested UI consistency across multiple device viewports simultaneously: iPhone 14 Pro, Pixel 7 Pro, iPhone 14 Pro Max, iPad Air.

**Screenshots:** `/screenshots/responsive-testing/`

**Bug found:** Floating action buttons ("Newsletter" and "VIP Concierge") overlap with image content in the "Exclusive Destinations" section on mobile viewports.

---

## 3. Bug Report Example (Jam.dev)

**Tool used:** [Jam](https://jam.dev)

**Title:** `[UI/Responsive] Los botones VIP Concierge y Newsletter se superponen con las imágenes en vista móvil.`

**Environment:**
- URL: https://exclusivesextocontinente.pages.dev/
- OS: Windows 11 (x86)
- Browser: Chrome 150.0.7871.129
- Window size: 1536x742
- Location: Peru

**Steps to Reproduce:**
1. Abrir la web en dispositivos móviles.
2. Hacer scroll hacia la sección "Exclusive Destinations".

**Expected Result:**
Los botones flotantes no deben tapar el texto ni los contenedores de imágenes.

**Actual Result:**
Los botones "Newsletter" y "VIP Concierge" se superponen con las imágenes de destinos.

**Screenshot / recording:** `/screenshots/bug-report/`

---

## 4. Tech Stack / Environment Analysis

**Tool used:** Wappalyzer
**Project:** Sexto Continente

Used to identify the technology stack running on a live site as part of exploratory testing (analytics, CDN, tag manager, JS libraries) — useful for understanding what tools may be involved when investigating bugs.

Detected: Google Analytics (GA4), Cloudflare (CDN), Sentry (error tracking), Google Tag Manager, Font Awesome, MobX.

**Screenshots:** `/screenshots/tech-stack/`

---

## 🎓 Currently Studying

- ISTQB Foundation Level (CTFL)
- SSTQB (Spanish Software Testing Qualifications Board)
- HASTQB (Hispanic America Software Testing Qualifications Board)

## 🛠️ Tools in this portfolio

`Thunder Client` · `Jira` (learning) · `Jam` · `Wappalyzer` · `Responsive Viewer`

---

*This portfolio is actively growing as I continue studying and practicing QA fundamentals. Open to entry-level remote QA / Software Tester opportunities.*
