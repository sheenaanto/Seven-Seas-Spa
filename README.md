# Seven Seas Spa

A simple static website showcasing spa services, built with HTML, Bootstrap 5, and minimal JavaScript. This repository provides an accessible and responsive layout for a spa treatment website with a clear services overview, contact form, and consistent header/footer.

---

## Live preview

- Open `index.html` directly in your browser, or
- Run a local web server (recommended for robust behavior)

---

## Features

- Responsive layout using Bootstrap 5
- Navigation with brand logo and links (Home, About, Services, Contact)
- Hero banner with overlay and vertical centering
- "Our Services" section with 4 service cards (image, heading, one-line description)
- Contact page with accessible contact form (client-side validation), redirects to `thankyou.html` on success
- Shared header and footer across pages for consistent UX
- Accessibility-focused elements: keyboard focusable nav, aria-labels, alt text, skip/main landmarks

---

## File structure

```
Seven-Seas-Spa/
├─ index.html            # Homepage (hero, services, testimonials)
├─ about.html            # About page (stub placeholder)
├─ services.html         # Services page (if present)
├─ contact.html          # Contact page with validated form
├─ thankyou.html         # Form success redirect page
├─ assets/
│  ├─ css/
│  │  └─ style.css       # Custom styles
│  ├─ images/            # Logo, hero, service images
│  └─ js/                # (Optional) site JS files
└─ README.md
```

---

## Run locally (Windows PowerShell)

1. Open PowerShell in the project root folder:

````

2. Start a quick static server with Python 3:

```powershell
python -m http.server 8000
````

3. Open http://localhost:8000 in your browser.

Tip: Install the "Live Server" extension in VS Code for a one-click local server and automatic reloads.

---

## Development notes

- This is a static HTML/CSS site. If you want to capture form submissions, add a server endpoint or use a third-party form provider.
- The contact form uses HTML5 validation and a small script in `contact.html` that calls `form.checkValidity()` and redirects to `thankyou.html` when valid.
- The "Our Services" cards currently use placeholder images; replace the `src` values in the `img` elements to show your own images in `assets/images/`.
- Change the hero height in `assets/css/style.css` under `.hero` — currently `min-height: 60vh` to adjust the banner appearance.

---

## Accessibility & Best Practices

- Ensure images have `alt` attributes.
- Keep the `aria-label` attributes for social links and toggles where appropriate.
- Use the `.was-validated` class on forms (Bootstrap) for better visual cues on invalid fields.

---

## Contributing

- Clone the repository, create a new branch, and send a pull request for review.

Example:

```powershell
git clone <repo-url>
cd Seven-Seas-Spa
git checkout -b feature/add-service-page
```

---
