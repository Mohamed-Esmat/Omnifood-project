# 🍽️ Omnifood Project

A responsive, modern landing page for a fictional AI-powered food delivery service, built using semantic HTML, custom CSS (Flexbox & Grid), and vanilla JavaScript. This project focuses on frontend development principles such as layout design, responsive behavior, and basic interactivity.

## 📚 Table of Contents

* [📖 Overview](#overview)
* [🛠️ Technologies Used](#technologies-used)
* [🚧 Challenges Faced](#challenges-faced)
* [📈 Learning Outcomes](#learning-outcomes)
* [📸 Screenshots](#screenshots)
* [📁 Directory Structure](#directory-structure)
* [🤝 Collaboration](#collaboration)
* [📬 Contact Me](#contact-me)

---

## 📖 Overview

Omnifood is a fictional food delivery platform that leverages AI to provide personalized meal recommendations. This project was created to practice real-world HTML and CSS skills, including responsive layout design, mobile-first development, and light JavaScript interactivity. The design is inspired by a Figma UI and was built to be fully functional on all screen sizes.

**🔗 Live Preview**: [View Website](https://omnifood-esmat.netlify.app/)

---

## 🛠️ Technologies Used

* **HTML5** – Semantic structure
* **CSS3** – Flexbox, Grid, Media Queries
* **JavaScript (ES6)** – For mobile navigation and sticky navbar
* **Intersection Observer API** – For sticky header behavior
* **Web Manifest** – For installable mobile app experience
* **Open Graph Meta Tags** – Basic SEO and social media preview
* **Netlify** – Deployment and custom domain linking

---

## 🚧 Challenges Faced

* **🎨 Design Translation**: This was the first time I translated a design from Figma to code, which improved my layout precision and structure.
* **📱 Responsive Design**: Implementing mobile and tablet responsiveness using media queries and layout techniques.
* **📌 Sticky Navigation**: Learned and used the Intersection Observer API to implement a sticky navigation bar that appears after scrolling past the hero section.
* **🧠 JavaScript Use**: Wrote minimal but effective JavaScript for toggling mobile navigation.

```js
const btnNav = document.querySelector(".btn-mobile-nav");
const headerEl = document.querySelector(".header");

btnNav.addEventListener("click", function () {
  headerEl.classList.toggle("nav-open");
});

const sectionHeroEl = document.querySelector(".section-hero");

const obs = new IntersectionObserver(
  function (entries) {
    const ent = entries[0];
    if (!ent.isIntersecting) document.body.classList.add("sticky");
    else document.body.classList.remove("sticky");
  },
  {
    root: null,
    threshold: 0,
    rootMargin: "-80px",
  }
);
obs.observe(sectionHeroEl);
```

---

## 📈 Learning Outcomes

* Developed a deep understanding of responsive web design using Flexbox, Grid, and media queries.
* Gained practical experience with semantic HTML and learned how it improves SEO and accessibility.
* Deployed a static website to Netlify and configured a custom domain.
* Learned about the web manifest and basic PWA features.

---

## 📸 Screenshots

## ![Preview Screenshot](https://res.cloudinary.com/tawfeer/image/upload/c_pad,w_1280/v1750145398/omnifood-website_j00whu.png)

---

## 📁 Directory Structure

```
.
├── content.md
├── css/
│   ├── general.css
│   ├── queries.css
│   └── style.css
├── img/
│   └── [... images for app, meals, gallery, logos, etc.]
├── js/
│   └── script.js
├── manifest.webmanifest
├── index.html
└── README.md
```

---

## 🤝 Collaboration

Feel free to contribute! If you find a bug, have a suggestion, or want to help improve the code:

1. 🍴 Fork the repository
2. 🌿 Create a new branch
3. ✏️ Make your changes
4. 📩 Submit a pull request

---

## 📬 Contact Me

If you have any questions or feedback, feel free to reach out:

* **📧 Email**: [msmt0452@gmail.com](mailto:msmt0452@gmail.com)
* **💻 GitHub**: [github.com/Mohamed-Esmat](https://github.com/Mohamed-Esmat)

---

© 2025 Mohamed Esmat. All rights reserved.
