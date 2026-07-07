# Bootstrap Internship Task

A responsive multi-page website built with **Bootstrap 5** as part of an internship assignment. The site showcases a fictional company called **RK Technology** and demonstrates modern web layout techniques using official Bootstrap components.

## Overview

This project is a static website with three pages — Home, About, and Contact. It uses Bootstrap's grid system, utility classes, and pre-built components to create a clean, mobile-friendly user interface without a backend or build step.

The design remixes patterns from Bootstrap's official examples (Heroes, Album, and Product layouts) and combines them into a cohesive business-style website.

## Live Preview

Open `index.html` in any modern web browser to view the site locally. No installation or server setup is required.

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

1. Clone or download this repository.
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

## Author

Built as a **Bootstrap Internship Task** for RK Technology.

## License

This project is created for educational and internship purposes.
