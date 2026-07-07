# Bootstrap Internship Task

A responsive multi-page website built with **Bootstrap 5** as part of an internship assignment. The site showcases a fictional company called **RK Technology** and demonstrates modern web layout techniques using official Bootstrap components.

## Links

- **GitHub Repository:** [github.com/Arpenaboyina/BootStrap_Task](https://github.com/Arpenaboyina/BootStrap_Task.git)
- **Live Preview (Netlify):** [quiet-brioche-656642.netlify.app](https://quiet-brioche-656642.netlify.app/)

## Overview

This project is a static website with three pages — Home, About, and Contact. It uses Bootstrap's grid system, utility classes, and pre-built components to create a clean, mobile-friendly user interface without a backend or build step.

The design remixes patterns from Bootstrap's official examples (Heroes, Album, and Product layouts) and combines them into a cohesive business-style website.

## Live Preview

- View the deployed site here: **https://quiet-brioche-656642.netlify.app/**
- Or open `index.html` in any modern web browser to view the site locally. No installation or server setup is required.

## Technologies Used

| Technology | Version | Purpose |
|------------|---------|---------|
| HTML5 | — | Page structure and content |
| Bootstrap | 5.3.7 | Responsive layout, components, and utilities |
| Bootstrap Icons | 1.11.3 | Icons for features, team, and social links |
| Custom CSS | `style.css` | Additional styling (referenced in all pages) |

All Bootstrap assets are loaded via CDN — no `npm install` or package manager is needed.

## Project Structure

```
Bootstrap-Internship-Task/
├── index.html      # Home page with hero, features, and call-to-action
├── about.html      # About page with mission, vision, and team section
├── contact.html    # Contact page with form and company details
├── style.css       # Custom styles (linked from all pages)
└── README.md       # Project documentation
```

## Pages

### Home (`index.html`)

- **Navbar** — Dark-themed responsive navigation with collapsible mobile menu
- **Hero section** — Headline, description, CTA button, and hero image
- **Features** — Three cards highlighting Web Development, Mobile Friendly, and Fast Performance
- **Call to action** — Primary-colored banner with a link to the Contact page
- **Footer** — Branding and social media icons

### About (`about.html`)

- **Intro section** — Brief company description
- **Mission & Vision** — Two side-by-side cards with icons
- **Team** — Three team member cards with profile images and roles

### Contact (`contact.html`)

- **Header banner** — Page title and subtitle
- **Contact form** — Fields for name, email, phone, subject, and message (frontend only; no submission backend)
- **Footer** — Company info, contact details, working hours, and social links

## Bootstrap Components Used

- Navbar with toggler (responsive collapse)
- Grid system (`container`, `row`, `col-*`)
- Cards with shadows
- Buttons (`btn`, `btn-primary`, `btn-light`)
- Forms (`form-control`, `form-label`)
- Typography utilities (`display-4`, `lead`, `fw-bold`)
- Spacing utilities (`py-5`, `mb-4`, `g-4`)
- Color utilities (`bg-dark`, `bg-primary`, `text-white`)
- Bootstrap Icons (`bi-laptop`, `bi-phone`, `bi-envelope-fill`, etc.)

## How to Run

1. Clone or download this repository:
   ```bash
   git clone https://github.com/Arpenaboyina/BootStrap_Task.git
   ```
2. Navigate to the project folder.
3. Open `index.html` in your browser (double-click the file or use **Open with Live Server** in VS Code).

Alternatively, serve the folder with a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (if npx is available)
npx serve .
```

Then visit `http://localhost:8000` in your browser.

## Responsive Design

The site is fully responsive:

- **Desktop** — Multi-column layouts for hero, features, and team sections
- **Tablet** — Grid columns adjust using Bootstrap's `col-md-*` breakpoints
- **Mobile** — Navbar collapses into a hamburger menu; content stacks vertically

## Notes

- The contact form is for display only. Submitting the form does not send data anywhere.
- External images are loaded from Unsplash and RandomUser.me.
- Ensure `style.css` exists in the project root for any custom styles referenced by the HTML files.

## Submission

- **GitHub Repository:** https://github.com/Arpenaboyina/BootStrap_Task.git
- **Live Deployed Link:** https://quiet-brioche-656642.netlify.app/

## Project Reflection

### How I approached the project

I started by going through the official [Bootstrap 5 Examples](https://getbootstrap.com/docs/5.3/examples/) to see how real Bootstrap components — navbars, hero sections, cards, and forms — are structured and styled. Rather than copying any single example page wholesale, I picked pieces I liked from different examples (the Album layout's card grid, the Hero layout's two-column intro, and a standard Bootstrap form) and combined them into three original pages for a fictional company, RK Technology:

1. **`index.html`** — Built the navbar first since it's shared across all pages, then added the hero section, a 3-card feature grid, a call-to-action banner, and a footer.
2. **`about.html`** — Reused the same navbar, then added a Mission/Vision card pair and a team section with profile cards.
3. **`contact.html`** — Built the contact form using Bootstrap's `form-control` and `form-label` utilities, then added a footer with contact details and working hours.

Once all three pages had a working first draft, I went back and adjusted spacing, colors, and typography utilities so the pages felt consistent rather than three separate designs.

### AI tools and external help used

In the interest of transparency: I built the pages myself using Bootstrap 5 and the official documentation as my main reference. While working on `contact.html`, I ran into a layout bug where the footer had gotten nested inside the contact form's column div instead of sitting as its own full-width section. After finding this bug, I used **ChatGPT** to help me understand and fix it — it helped identify the mismatched `<div>` nesting and how to restructure the closing tags so the footer would render correctly, full-width, below the form section.

Outside of that specific bug fix, the component selection, layout decisions, and content (copy, section order, styling choices) across all three pages were done by me using the official Bootstrap documentation as the primary reference.

### Challenges faced

- **Layout/markup bugs:** The trickiest issue was a mismatched `<div>` nesting in the contact page that caused the footer to render inside the form's column instead of full-width. I caught this by reviewing the rendered layout and fixed it by restructuring the closing tags so the footer sits outside the `<section>` as its own block.
- **Consistency across pages:** Since each page was built somewhat independently, keeping the navbar, footer, and spacing consistent across all three took a second pass of comparison and cleanup.
- **Form without a backend:** Since this is a static site with no server, the contact form doesn't actually send data anywhere yet — I noted this clearly rather than implying it works end-to-end.

### Learning journey

This task pushed me to actually read Bootstrap's component documentation rather than just recognizing class names, and to think about layout composition (how a hero, feature grid, and CTA band flow into each other) rather than treating each component in isolation. Debugging the div-nesting issue also reinforced why consistent indentation and closing tags matter, especially in nested Bootstrap grid structures (`container` → `row` → `col`).

