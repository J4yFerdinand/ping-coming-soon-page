# Ping – Coming Soon Page 🎉

A clean, responsive “coming soon” landing page for the fictional Ping service. Built as part of the [Frontend Mentor](https://www.frontendmentor.io/) challenge.

![Project preview](./preview.jpg)

---

## Table of Contents
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Folder Structure](#folder-structure)
- [What I Learnt](#what-i-learnt)
- [Author](#author)
- [Acknowledgements](#acknowledgements)

---

## Features
- Mobile-first, fully responsive layout (375 px → 1440 px)
- Interactive email subscription form
  - Red outline + inline error message if input empty or invalid (uses a **single** RegExp)
  - Green/blue outline and cleared field on success
- Subtle hover/active states for all interactive elements
- Accessible markup (`label`, `button`, `aria-` attributes) and semantic HTML5

---

## Tech Stack
- Semantic **HTML5**
- **CSS3** with custom properties, Flexbox & media queries
- Vanilla **JavaScript** (≈20 LOC) for validation
- No build tools or frameworks – just open the file and go!

---

## Getting Started
1. Clone the repo  
   ```bash
   git clone https://github.com/J4yFerdinand/ping-coming-soon-page.git
   cd ping-coming-soon-page
   ```
   
2. Open _**index.html**_ in your browser (double-click or serve locally).
"_Optional: Use a simple dev server such as VS Code Live Server for hot-reload._"

## Folder Structure
```
ping-coming-soon-page-master
├── design/              # Challenge reference designs
├── images/              # Optimised PNG/SVG assets
├── index.html
├── styles.css
├── main.js              # Email validation logic
├── preview.jpg          # README/OG image
└── style-guide.md       # Colours, fonts & spec from challenge
```

---

## What I Learnt
- Crafting a RegExp that covers most valid/invalid email cases while remaining readable:

```js
let regExp =
  /[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*@(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?/g
```

- Using `preventDefault()` to stop a form submission while still validating.
- Quick, responsive layouts with ***min/max width containers and utility classes***.

---
## Author
- [Github](https://github.com/J4yFerdinand/)
- [LinkedIn](https://www.linkedin.com/in/joferiva/)

---
## Acknowledgements
Huge thanks to Frontend Mentor for the design and challenge brief, and to the dev community for constant inspiration. 🚀