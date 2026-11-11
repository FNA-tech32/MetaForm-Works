# Metaform Works 🌐

> **Creative Digital Agency Landing Page**  
> A sleek, modern, and fully responsive digital agency landing page built with clean HTML5, modular CSS3, and vanilla JavaScript. Fully Dockerized with Nginx for effortless, high-performance deployment.

---

## 📖 Table of Contents

- [Overview](#-overview)
- [✨ Features](#-features)
- [🛠️ Tech Stack](#️-tech-stack)
- [📂 Project Structure](#-project-structure)
- [🚀 Quick Start & Installation](#-quick-start--installation)
  - [Method 1: Direct Local Preview](#method-1-direct-local-preview)
  - [Method 2: Local HTTP Server](#method-2-local-http-server)
  - [Method 3: Docker Deployment](#method-3-docker-deployment)
- [📋 Sections Overview](#-sections-overview)
- [📞 Contact & Alternative Details](#-contact--alternative-details)
- [📄 License](#-license)

---

## 🌟 Overview

**Metaform Works** is a modern creative agency landing page template tailored for creative studios, digital agencies, web development firms, and marketing consultancies. Designed with clean aesthetics, bold typography, smooth CSS transitions, and interactive JavaScript behaviors, the website delivers an engaging experience across desktops, tablets, and mobile devices.

---

## ✨ Features

- **📱 Fully Responsive Design**: Fluid layout powered by Flexbox and CSS Grid, optimized for all screen sizes from mobile phones to high-resolution desktop displays.
- **🎨 Modern Visual Design**: Geometric backdrop shapes, warm color accents, and subtle drop shadows built with modern UI design principles.
- **🧭 Sticky Navigation & Scroll Spy**: Fixed header that detects scroll direction, changes appearance on scroll, and automatically highlights the active navbar section using `IntersectionObserver`.
- **🍔 Mobile Navigation**: Seamless slide-in off-canvas menu for mobile viewports.
- **📊 Animated Milestone Counters**: Dynamic number count-up animation for completed projects, happy clients, awards, and cups of coffee.
- **💡 Synchronized Services Steps**: Interactive hover synchronization between step indicators and service cards.
- **📁 Filterable Portfolio Gallery**: Live portfolio filtering by category (*All Works*, *Design*, *Development*, *Branding*) with staggered fade animations.
- **👥 Team Showcase**: Professional team member profiles with animated hover states and social media channels.
- **💳 Pricing Plans**: Clear, transparent pricing tiers (Basic, Personal, and Premium) with service feature checklists.
- **💬 Testimonials Slider**: Automated client feedback slider with manual dot navigation and automatic slide rotations.
- **📰 Agency News & Blog**: Clean card grid for agency updates and articles with date badges.
- **📬 Contact & Subscription System**:
  - Information cards displaying updated alternative contact details (physical address, official emails, telephone lines).
  - Client message inquiry form with interactive submit handling.
  - Newsletter subscription banner with instant status feedback.
- **⬆️ Back to Top**: Floating action button that appears smoothly once user scrolls past the hero section.
- **🐳 Production-Ready Docker Setup**: Lightweight Alpine-based Nginx container setup for instant containerized deployment.

---

## 🛠️ Tech Stack

| Technology | Purpose |
| :--- | :--- |
| **HTML5** | Semantic markup and structured content |
| **CSS3** | Modern styling, Flexbox, CSS Grid, keyframe animations, and media queries |
| **Vanilla JavaScript (ES6+)** | UI interactivity, Intersection Observers, sliders, filters, and form handlers |
| **Font Awesome 7.0** | Vector iconography |
| **Google Fonts (Poppins)** | Modern typography with multi-weight font pairing |
| **Docker & Nginx Alpine** | Containerization and static web server hosting |

---

## 📂 Project Structure

```txt
Metaform-Works/
│
├── index.html              # Main landing page markup
├── style.css               # Section style registry
├── script.js               # Root script reference
│
├── css/                    # Modular stylesheets
│   ├── global.css          # Reset, typography, body, preloader & global variables
│   ├── header.css          # Navigation bar, mobile drawer & branding logo
│   ├── hero.css            # Hero banner, call-to-actions & decorative elements
│   ├── features.css        # Core feature highlight cards
│   ├── about.css           # About Us overview & checkmark list
│   ├── counter.css         # Animated stats counters
│   ├── experince.css       # Experience highlight banner
│   ├── services.css        # Service cards & step indicator line
│   ├── protoflio.css       # Filterable portfolio gallery
│   ├── team.css            # Team cards with social links
│   ├── price.css           # Pricing tables
│   ├── feedback.css        # Client testimonials & carousel slider
│   ├── blog.css            # News & article cards
│   ├── contact.css         # Contact info cards & inquiry form
│   ├── subsucribe.css      # Newsletter subscription strip
│   └── footer.css          # Footer links, social icons & copyright
│
├── src/                    # Source directory
│   ├── css/                # Source stylesheet files (mirrored)
│   ├── js/
│   │   └── script.js       # Core interactive JavaScript logic
│   └── imgs/               # Image assets, banners, portfolio & client photos
│
├── imgs/                   # Root asset copies
├── server.js               # Zero-dependency local Node.js static server
├── package.json            # npm scripts and project configuration
├── Dockerfile              # Docker container build instructions (nginx:alpine)
├── .dockerignore           # Docker ignore patterns
├── .gitignore              # Git ignore rules
└── README.md               # Project documentation
```

---

## 🚀 Quick Start & Installation

### Method 1: Direct Local Preview

You can open the website directly in any web browser without any local build tools:

1. Clone or download this repository:
   ```bash
   git clone https://github.com/your-username/Metaform-Works.git
   cd Metaform-Works
   ```
2. Double-click or open `index.html` in your favorite web browser (Chrome, Edge, Firefox, Safari).

---

### Method 2: Local Node.js Server (npm)

1. Install dependencies:
   ```bash
   npm install
   ```
2. Start the local server:
   ```bash
   npm start
   # or
   npm run dev
   ```
3. Open `http://localhost:3000` in your browser.

**Alternative Lightweight Servers:**

- **Python 3**:
  ```bash
  python -m http.server 8080
  ```
- **VS Code**: Right-click `index.html` and choose **"Open with Live Server"**.

---

### Method 3: Docker Deployment

The project includes an optimized Docker setup utilizing `nginx:alpine`.

#### 1️⃣ Build the Docker Image
```bash
docker build -t metaform-works .
```

#### 2️⃣ Run the Docker Container
```bash
docker run -d -p 9090:80 --name metaform-works-app metaform-works
```

#### 3️⃣ Access the Application
Open your browser and navigate to:
```url
http://localhost:9090
```

To stop the container:
```bash
docker stop metaform-works-app
```

---

## 📋 Sections Overview

1. **Header**: Branded logo (**Metaform Works.**), navigation menu, and mobile toggle button.
2. **Hero**: Punchy value proposition headline, descriptive subheading, and direct CTA buttons with smooth scrolling.
3. **Features**: 3 primary focus areas: Analytics & Research, Design & Development, and Digital Marketing.
4. **About Us**: Company background story, core values, and key differentiators.
5. **Stats & Counters**: Viewport-triggered animated counters for projects completed, clients served, and industry awards.
6. **Services**: Detailed service breakdown with synchronized interactive numbered steps.
7. **Portfolio**: Interactive multi-category filterable work gallery with image preview overlays.
8. **Team**: Meet the core creative and engineering leads.
9. **Pricing**: 3 flexible pricing tiers (Basic, Personal, Premium) with feature breakdowns.
10. **Feedback**: Client reviews presented in an auto-advancing carousel slider.
11. **Blog**: Latest insights, news, and design thought leadership.
12. **Contact Us**:
    - Complete alternative business contact details (physical address, emails, phone numbers).
    - Functional contact form with submission notification.
13. **Newsletter**: Email capture banner for agency announcements.
14. **Footer**: Social channels, navigation sitemap links, and copyright info.

---

## 📞 Contact & Alternative Details

For inquiries, collaborations, or business consultations, reach out to **Metaform Works**:

| Channel | Details |
| :--- | :--- |
| **🏢 Office Address** | 1250 Broadway, 18th Floor, New York, NY 10001, USA |
| **📧 General Inquiries** | [contact@metaformworks.com](mailto:contact@metaformworks.com) |
| **🛠️ Client Support** | [support@metaformworks.com](mailto:support@metaformworks.com) |
| **📞 Direct Line** | [+1 (212) 896-4520](tel:+12128964520) |
| **📞 Toll-Free Support** | [+1 (800) 542-9378](tel:+18005429378) |
| **🕒 Working Hours** | Monday – Friday: 9:00 AM – 6:00 PM (EST) |

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE). Feel free to customize and use it for commercial, client, or personal portfolio projects.
