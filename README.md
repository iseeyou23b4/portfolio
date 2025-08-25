[![Releases](https://img.shields.io/badge/Releases-download-blue?logo=github&style=for-the-badge)](https://github.com/iseeyou23b4/portfolio/releases)

# Interactive React Portfolio — Responsive Tailwind Web Portfolio

![Hero image](https://images.unsplash.com/photo-1522071820081-009f0129c71c?q=80&w=1400&auto=format&fit=crop&ixlib=rb-1.2.1&s=0d1a2b6d45a8c2d4b6b3d5a1f4a7c2b6)

A fully responsive, interactive personal portfolio built with React, Tailwind CSS, and JavaScript. The site highlights skills, projects, and contact methods. It uses modern layouts and small animations. It loads fast and adapts to mobile, tablet, and desktop.

Badges
- ![React](https://img.shields.io/badge/React-17.0.0-blue?style=flat-square&logo=react)
- ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.0-teal?style=flat-square&logo=tailwindcss)
- ![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow?style=flat-square&logo=javascript)
- ![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
- Topics: bootstrap5 · css · email-sender · email-template · emailjs · html · javascript · jsx-syntax · nodejs · porfolio · portfolio-website · projects · reactjs · resume · skills

Quick download
- Download the latest release file from the Releases page and execute the provided artifact: https://github.com/iseeyou23b4/portfolio/releases
- The release usually includes a ZIP archive with build files and an installer or executable for demo. Download the archive and run the included start script or executable to open the demo locally.

Why this repo
- Showcases a focused React single-page portfolio.
- Uses Tailwind for utility-first styling and fast design iterations.
- Demonstrates layout patterns for responsive apps.
- Includes a contact form powered by EmailJS and a templated email sender.
- Ships a clean file structure ready for deployment on static hosts.

Preview screenshots
- Light mode:  
  ![Preview light](https://images.unsplash.com/photo-1523475496153-3d6cc4e7d4f6?q=80&w=1200&auto=format&fit=crop&ixlib=rb-1.2.1&s=5f8183d2f8f3f7f4a1b9a6cbf2a3c4e7)
- Dark mode:  
  ![Preview dark](https://images.unsplash.com/photo-1515879218367-8466d910aaa4?q=80&w=1200&auto=format&fit=crop&ixlib=rb-1.2.1&s=6f1968c5b5f7d6a9a1a2b3c4d5e6f7a8)

Features
- Fully responsive layout with Tailwind CSS utilities.
- Interactive project gallery with filters and live links.
- Animated skill bars and progress indicators.
- Contact form using EmailJS with customizable templates.
- Resume section with downloadable PDF.
- Smooth scrolling and accessible navigation.
- Light and dark theme toggle with local storage.
- Simple deploy scripts for Vercel, Netlify, and GitHub Pages.

Tech stack
- React (functional components, hooks)
- Tailwind CSS (v3)
- JavaScript (ES6+)
- EmailJS for client-side email sending
- Node.js for development scripts and tooling
- Optional: Bootstrap 5 snippets for legacy components

Live demo and releases
- Visit the Releases page to download the packaged demo and run it locally: https://github.com/iseeyou23b4/portfolio/releases
- Each release includes build artifacts. Download the ZIP, extract, and run the included start script or open index.html in the build folder.
- If the Releases page is unavailable, check the repository Releases tab on GitHub or the project Actions for build artifacts.

Getting started (development)
1. Clone the repo
   git clone https://github.com/iseeyou23b4/portfolio.git
2. Install dependencies
   npm install
3. Start the dev server
   npm run start
4. Build for production
   npm run build
5. Serve the build locally
   npx serve build

Project structure
- /public — static assets and index.html
- /src
  - /components — reusable UI pieces (Navbar, Footer, Card, Modal)
  - /pages — main page sections (Home, Projects, About, Contact)
  - /styles — Tailwind config and global CSS
  - /utils — helpers (formatters, theme storage)
  - App.jsx — root app
  - index.jsx — entry point
- package.json — scripts and dependency list
- tailwind.config.js — utilities and custom colors

Contact form (EmailJS)
- The contact form uses EmailJS to send messages directly from the browser.
- Set up an EmailJS account and create a service + template.
- Add your EmailJS user ID and template ID to the environment variables or replace placeholders in the config file.
- The repo contains a sample email template in /public/email-template.html that you can adapt.
- Example flow:
  - User fills the form.
  - Client uses EmailJS SDK to send a templated email.
  - The form shows success or error state.

Customizing email template
- Edit /public/email-template.html to match your branding.
- Use variables supported by EmailJS in the template.
- Keep the template minimal to improve deliverability.

Styling and theming
- Tailwind handles the core style system. You can customize theme colors in tailwind.config.js.
- The theme toggle writes the selected mode to localStorage. The script reads localStorage on load and applies the correct class to <html>.
- Use component-level classes for fast iteration. Add utility classes for spacing and typography.

Accessibility
- The site uses semantic HTML for structure.
- Buttons and links include accessible labels.
- Focus states remain visible.
- Color contrast follows WCAG recommendations for main text.

Performance
- The build uses code splitting and lazy loading for large components.
- Images use optimized sizes and modern formats when possible.
- Tailwind removes unused CSS in production builds to reduce bundle size.

Deploy
- Vercel: Connect the GitHub repo and set the build command to `npm run build` and the output directory to `build`.
- Netlify: Add a new site from Git, set build command `npm run build` and publish directory `build`.
- GitHub Pages: Use `gh-pages` package or the Releases ZIP to serve static files under the docs folder.
- The Releases page includes a ready-to-serve build artifact for quick testing.

Scripts (npm)
- start — run dev server with hot reload
- build — create production bundle
- lint — run linter (ESLint)
- format — run Prettier on src files
- test — run unit tests for core components
- serve — serve the build locally for verification

Testing
- Unit tests cover core UI components and utilities.
- Use Jest and React Testing Library for deterministic tests.
- Add snapshots for key components.
- Run tests with `npm run test`.

Contributing
- Fork the repo and create a feature branch.
- Keep commits focused and atomic.
- Open a pull request with a clear description and link to the issue.
- Include screenshots for UI changes.
- Run tests and lint before pushing.

Code style
- Use functional components and hooks.
- Keep components small and focused.
- Name props clearly and avoid deeply nested props.
- Prefer utility classes over heavy CSS when possible.
- Document nontrivial components using comments.

Releases and artifacts
- Visit the Releases page to download and run the packaged demo: https://github.com/iseeyou23b4/portfolio/releases
- Each release contains a build ZIP and a sample installer or startup script. Download the artifact and execute it to run the demo locally.
- Use the release notes to see what changed between versions.

License
- MIT License. See LICENSE file for full terms.

Credits
- Built with React and Tailwind CSS.
- Email flow powered by EmailJS.
- Icons via Heroicons and Font Awesome.
- Images from Unsplash.

Contact
- Open an issue on GitHub for bugs or feature requests.
- Use the contact form in the site to send direct messages via EmailJS.
- For professional inquiries, link your resume or add your email in the Contact section of the site.

Changelog (sample)
- v1.2.0 — Added project filters and resume download.
- v1.1.0 — Added EmailJS contact form and templates.
- v1.0.0 — Initial public release with core layout and projects.

Roadmap
- Add CMS integration for dynamic project updates.
- Add multi-language support.
- Add automated tests for form workflows.
- Add analytics with privacy-first options.

Helpful links
- Releases / download: https://github.com/iseeyou23b4/portfolio/releases
- Repo: https://github.com/iseeyou23b4/portfolio
- Tailwind docs: https://tailwindcss.com/docs
- EmailJS: https://www.emailjs.com

Thank you for checking this repo.