# Learnify

A static marketing website for an online education platform offering courses in web development, data science, AI/ML, cybersecurity, UI/UX design, and business.

**Live Site:** Deployed via GitHub Pages from the `main` branch.

## Tech Stack

- **HTML5** -- Semantic, multi-page structure
- **CSS3** -- Custom stylesheets with responsive design (5 breakpoints: 1024px, 992px, 768px, 640px, 480px)
- **Vanilla JavaScript** -- Minimal usage for password strength meter and form stubs
- **Font Awesome 6.5.1** -- Icons via CDN
- **Images** -- Externally hosted (Unsplash)

No frameworks, bundlers, or build tools are used.

## Pages

| Page | File | Description |
|------|------|-------------|
| Homepage | `index.html` | Landing page with hero, features, pricing, courses, testimonials |
| Courses | `coursepage.html` | Course catalog with category filters and course cards |
| About Us | `aboutus.html` | Mission, values, and instructor profiles |
| Contact | `contactus.html` | Contact form, support channels, and FAQ |
| Login | `login.html` | Sign-in page with social login options |
| Signup | `signup.html` | Registration page with password strength meter |
| Privacy Policy | `PrivacyPolicy.html` | Privacy policy with sticky table of contents |
| Refund Policy | `RefundPolicy.html` | Refund policy and process |
| Terms & Conditions | `TermsAndConditions.html` | Terms of service |

## Project Structure

```
.
├── .github/workflows/
│   └── jekyll-gh-pages.yml    # GitHub Pages deployment workflow
├── index.html                 # Homepage
├── style.css                  # Global/shared stylesheet
├── coursepage.html            # Course catalog
├── coursepage.css
├── aboutus.html               # About Us
├── aboutus.css
├── contactus.html             # Contact Us
├── contactus.css
├── login.html                 # Sign in
├── login.css
├── signup.html                # Registration
├── signup.css
├── PrivacyPolicy.html         # Privacy Policy
├── PrivacyPolicy.css
├── RefundPolicy.html          # Refund Policy
├── RefundPolicy.css
├── TermsAndConditions.html    # Terms & Conditions
└── TermsAndConditions.css
```

Each page loads `style.css` (global styles, header, footer, resets) alongside its own page-specific CSS file.

## Running Locally

No installation is required. Open any `.html` file directly in a browser, or use a local static server:

```bash
# Using Python
python3 -m http.server 8000

# Using Node.js
npx serve .
```

Then visit `http://localhost:8000`.

## Deployment

The site deploys automatically to GitHub Pages on every push to `main` via the workflow at `.github/workflows/jekyll-gh-pages.yml`.

## Key Features

- Fully responsive layout across mobile, tablet, and desktop
- 4-tier pricing section (Starter, Standard Pro, Premium Master, Enterprise)
- Course catalog with category filters and detailed course cards
- Instructor profiles with social links
- Student testimonials with ratings
- FAQ accordion using native `<details>`/`<summary>` elements
- Split-screen authentication pages with social login buttons
- Legal pages with sticky sidebar navigation

## Notes

- All forms are front-end only -- no backend or API integration exists
- Interactive elements (filters, sort, pagination, billing toggle) are visual placeholders
- All images are loaded from external URLs (no local image assets)
