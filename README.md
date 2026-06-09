# InAmigos Foundation — Interactive Awareness Portal

A premium, modern, and fully responsive tab-based awareness webpage designed for the **InAmigos Foundation** (a Section 8 non-profit organization). This portal serves as a comprehensive hub showcasing the foundation's initiatives, social impact, credentials, campaign gallery, and latest blogs.

Designed with a **Light Glassmorphism** theme, it combines soft gradients, frosted panels, and smooth micro-animations to offer a modern web experience.

---

## 🚀 Key Features

### 1. Single Page Application (SPA) Tabbed Flow
*   **Home**: Includes a stunning Hero section, **Floating Quick Actions overlay cards** (Donate, Volunteer, Join), Strategic Pillars, InAmigos Operations Timeline, Campaign Highlights, and an interactive **Events Grid** (World Water Day 2025, Day of Happiness 2025, Women in Science 2025).
*   **About Us**: Explains the organization's founding history under Founder Mr. Govind Shukla, official Central Government Section 8 licenses, tax-exempt certifications (80G & 12A), CSR-1 registration, and detailed key initiatives impact lists.
*   **Our Projects**: Interactive cards for the 6 core initiatives:
    *   *Project SEVA* (Nutrition Security)
    *   *Project BACHPANSHALA* (Educational Micro-Hubs)
    *   *Project JEEV* (Stray Animal Welfare)
    *   *Project UDAAN* (Women Empowerment & Health)
    *   *Project PRAKRITI* (Eco-Conservation)
    *   *Project VIKAS* (Professional Skills Internships)
*   **Project Details Tab**: A dynamic, JavaScript-powered sub-page displaying rich media details and metrics for any clicked project without page reloads.
*   **Activity Gallery**: A responsive masonry-like photo grid containing actual campaign photos.
*   **Latest Blogs**: An interactive dashboard showing 10 official InAmigos articles with filter tags.
*   **Get Involved**: Clear calls-to-action to register as a volunteer, intern, or donor.

### 2. Premium Design & Micro-Animations
*   **Frosted Glass System**: Utilizes `backdrop-filter: blur` styling paired with harmonious HSL tailwind-inspired colors (Mint, Sage, Forest Green).
*   **Stats Count-Up Animation**: Dynamic numbers count up in real-time when scrolling into the viewport.
*   **Scroll Reveal Transitions**: Elements fade and lift up smoothly as they enter the screen using a high-performance `IntersectionObserver`.
*   **Ambient Background Orbs**: Soft colored background bubbles follow the mouse pointer with a parallax effect.
*   **Dynamic Lightbox Modal**: Clicking any image in the Gallery triggers a full-screen blurred lightbox modal with left/right keyboard navigation support.

---

## 📂 Project Structure

```
Task 1/
├── Elsie/             # Local display typography files
├── Images/            # Visual assets & icons
│   ├── Gallery/       # Photos for the Activity Gallery grids
│   ├── Project/       # Cover photos for campaigns and blog posts
│   ├── Logo.jpg       # Brand logo image
│   ├── landimg.jpg    # Landing page hero background banner
│   └── about.jpg      # Section branding imagery
├── Reference_design/  # Reference layout mockups
├── index.html         # Main markup layout, tab containers, and SPA triggers
├── style.css          # Extracted stylesheet (design system, grid styles, scroll reveal)
└── README.md          # Project documentation (this file)
```

---

## 🛠️ Installation & Running Locally

Since the application uses relative paths to load the local images folder outside of the `Task 1` directory, you should spin up a local server from the **workspace root directory** to prevent `404 Not Found` errors:

1.  Open your terminal in the workspace root directory:
    ```bash
    cd "InAmigos foundations"
    ```
2.  Start a local development server (Python is installed on most systems):
    ```bash
    python -m http.server 8000
    ```
3.  Open your browser and navigate to:
    ```
    http://localhost:8000/Task 1/index.html
    ```

---

## 🎨 Technology Stack
*   **Structure**: Semantic HTML5 (header, section, nav, main, footer)
*   **Styling**: Modern CSS3 (Custom properties design tokens, CSS Grid/Flexbox layouts, `@media` responsive breakpoints, `@keyframes` keyframe transitions)
*   **Logic**: Pure Vanilla Javascript ES6+ (no external frameworks like React/Angular required)
*   **Icons**: FontAwesome v6.4 (linked via CDN)
*   **Typography**: Google Fonts (*Elsie* for headings & *DM Sans* for body copy)
