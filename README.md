# 🍳 Anyone Can Cook — HR Website Guide

This repository contains the source code for the **Anyone Can Cook (ACC)** Careers Website.  
It serves as the main HR site where applicants can learn about our brands and submit their applications.

---

## 🗂️ Structure Overview

The site has **three main pages** located in the `/` directory:

| File | Description |
|------|--------------|
| `index.html` | Homepage — features the Anyone Can Cook logo and the three brands (Purple Oven, Goffa, and Village Cook). |
| `careers.html` | Careers Page — lists job openings and includes an **Apply Now** button for each role. |
| `apply.html` | Apply Now Page — shows instructions and requirements for applicants before submitting. |
| `style.css` | Main stylesheet controlling all colors, layout, and responsiveness. |
| `script.js` | JavaScript file for the mobile hamburger menu and small interactive features. |
| `/images` | Folder for all brand logos and related visuals. |

---

## 🧾 Editing the Website

### 1. Editing Text or Content
To update words, job listings, or descriptions:
1. Open the relevant `.html` file (for example, `careers.html`).
2. Look for the section you want to edit — it’s clearly labeled in comments (`<!-- like this -->`).
3. Update the text between the `<p>`, `<h2>`, or `<li>` tags.
4. Save the file and commit your changes.

💡 **Tip:**  
Use a simple text editor (VS Code, Sublime, or even GitHub’s built-in editor) to make small text edits.

---

### 2. Adding or Removing Job Openings
1. Open `careers.html`.
2. Each job posting is inside a `<div class="job">` block.
3. Copy one of the existing job blocks and paste it below to add a new one.
4. Update:
   - Job Title (`<h3>`)
   - Description (`<p>`)
   - The “Apply Now” button (no need to change the link, it’s automatic).

---

### 3. Changing the Apply Email
If the HR email ever changes:
1. Open `script.js`.
2. Find this line:
   ```js
   const hrEmail = "hrpurpleoven2@gmail.com";
