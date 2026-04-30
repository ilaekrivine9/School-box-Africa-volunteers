# School Box Africa - Volunteer Portal

A clean, single-page volunteer signup portal for [School Box Africa](https://schoolboxafrica.org) — an education technology startup building AI-powered shipping container learning labs across Africa to deliver vocational courses in agriculture, electrics, basic engineering, and more.

![School Box Africa Logo](public/logo.jpg)

## Features

- **Volunteer Application Form** — Collects full name, skills & experience, preferred contact method, and portfolio uploads
- **Contact Method Selection** — Volunteers choose between Email or WhatsApp; only the selected method is stored
- **Portfolio Uploads** — Support for PDF file uploads (drag & drop) and up to 3 URL links
- **Email Notifications** — Form submissions are sent to `schoolboxafrica@gmail.com` via Formspree
- **Responsive Design** — Works beautifully on mobile, tablet, and desktop
- **Accessible** — Proper labels, focus states, and ARIA attributes throughout

## Tech Stack

- [React](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/) + [Vite](https://vitejs.dev/)
- [Tailwind CSS](https://tailwindcss.com/) for styling
- [shadcn/ui](https://ui.shadcn.com/) components
- [GSAP](https://greensock.com/gsap/) for entrance animations
- [Lucide React](https://lucide.dev/) for icons
- [Formspree](https://formspree.io/) for form submission & email notifications

## Getting Started

### Prerequisites

- Node.js 18+ and npm

### Installation

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/sba-volunteer-portal.git
cd sba-volunteer-portal

# Install dependencies
npm install

# Start the development server
npm run dev
```

The app will be available at `http://localhost:5173`.

### Building for Production

```bash
npm run build
```

The built files will be in the `dist/` directory.

## Email Setup

This project uses [Formspree](https://formspree.io/) to handle form submissions and send email notifications.

1. Create a free account at [formspree.io](https://formspree.io/)
2. Create a new form
3. Replace the `FORMSPREE_ENDPOINT` in `src/App.tsx` with your form's endpoint URL
4. Update the form's notification email to `schoolboxafrica@gmail.com` in your Formspree dashboard

The free tier includes 50 submissions per month.

## Customization

### Colors

The brand colors are defined in `src/index.css` and `src/App.tsx`:

- Primary Blue: `#0057A4`
- Primary Hover: `#004B8D`
- Success Green: `#10B981`
- Error Red: `#EF4444`

### Logo

Replace `public/logo.jpg` with your own logo image.

## Project Structure

```
sba-volunteer-portal/
├── public/
│   ├── logo.jpg              # SBA logo
│   ├── sba-container-ai.jpg  # Branding images
│   ├── sba-exterior.jpg
│   ├── sba-interior-1.jpg
│   ├── sba-interior-2.jpg
│   └── sba-interior-3.jpg
├── src/
│   ├── App.tsx               # Main application component
│   ├── main.tsx              # Entry point
│   ├── index.css             # Global styles & theme
│   └── ...
├── index.html
├── package.json
├── tailwind.config.js
├── vite.config.ts
└── README.md
```

## Deployment

### Static Hosting (Free Options)

This is a static site that can be deployed anywhere:

- **[GitHub Pages](https://pages.github.com/)** — Free, built-in with GitHub
- **[Netlify](https://www.netlify.com/)** — Free tier with drag-and-drop deploy
- **[Vercel](https://vercel.com/)** — Free tier with Git integration
- **[Cloudflare Pages](https://pages.cloudflare.com/)** — Free with unlimited bandwidth

### Deploy to GitHub Pages

```bash
# Build the project
npm run build

# The dist/ folder contains the deployable files
# Follow GitHub Pages instructions to deploy the dist folder
```

## License

This project is open source and available under the [MIT License](LICENSE).

## About School Box Africa

School Box Africa builds AI-powered shipping container learning labs that deliver vocational education to developing communities across Africa. Courses cover practical skills like agriculture, electrics, basic engineering, and sustainable resource management.

Want to volunteer? Visit our portal and share your skills!

---

Made with care for communities across Africa.
