# Aatral Safetizen™ - XR Safety Training Platform

A modern, responsive product page for Aatral Safetizen™, an enterprise XR safety training platform featuring 21+ ready-to-deploy VR safety modules. Built with React, Vite, and TailwindCSS.

## 🌟 Overview

**Aatral Safetizen™** is part of Aatral's comprehensive enterprise XR training platform suite, providing immersive VR safety training modules for Manufacturing, Infrastructure, and Corporate environments.

### Key Features
- **21+ VR Safety Modules** - Ready-to-deploy training across General Safety, Killer Risk Safety, and EOT Crane Simulators
- **Multilingual Support** - All modules available in English and Hindi
- **3 Learning Modes** - Guided, Quiz, and Assessment for measurable competency
- **Industry-Specific** - Tailored for Manufacturing, Infrastructure, and Corporate sectors
- **Meta Quest Compatible** - Optimized for Meta Quest 3 and Meta Quest 3S

## 🎯 Product Page Sections

### 1. Hero Section
- **Compelling Value Proposition** - "Deploy 21+ ready-to-use VR safety modules in days, not months"
- **Trust Signals** - "Trusted by 50+ Global Enterprises"
- **Clear CTAs** - "Book Free VR Demo" and "Browse 21+ Modules"
- **Key Benefits** - Deploy in 48 Hours, Measurable Results, Multilingual Support
- **Social Proof** - 500+ safety professionals trained this month, 4.9/5 rating
- **Stats Showcase** - 21+ Modules, 3 Learning Modes, Multi Languages, Quest 3/3S support

### 2. Interactive Module Library
- **21+ Training Modules** organized by category:
  - Office Safety
  - Excavation Safety
  - PPE Orientation
  - Hot Works
  - Electrical Safety
  - Work At Height
  - Fire Safety
  - Chemical Safety
  - Environmental Safety
  - CPR Training
  - Shop Floor Safety

#### Filtering System
- **Search** - Real-time search by module name
- **Category Filter** - Mobile dropdown (< 640px), Desktop buttons (≥ 640px)
- **Language Filter** - English, Hindi, All languages
- **Runtime Filter** - ≤10 mins, >10 mins, All durations

#### Module Details Modal
- **Optimized Layout** - Inline labels for short fields, stacked for long content
- **Mobile-Friendly** - No scrolling required on mobile devices
- **Complete Information** - Category, Description, Learning Objective, Runtime, Languages, Industries, Devices
- **Video Integration** - Direct links to module demo videos

### 3. About Aatral Safetizen™
- Executive summary of the platform
- Key statistics and capabilities
- Industry applications

### 4. EOT Crane Simulators
- Dedicated cabin and pendant crane modules
- Steel plant and heavy manufacturing focus
- Realistic slab, billet, coin, and hot metal handling environments

### 5. Why Enterprises Choose Aatral Safetizen™
- **Real-world Risk Replication** - High fidelity scenarios mapped to Life Saving Rules
- **Assessment & Benchmarking** - Measurable competency scores
- **Hardware Integration** - Seamless peripheral support

### 6. Roadmap
- Upcoming modules: Chemical Safety, Material Handling, Shop Floor Safety
- Timeline: December 2025

### 7. Trusted By Industry Leaders
- **Infinite Logo Carousel** - 31 company logos including Tata, L&T, JSW, Indian Armed Forces
- **Smooth Animation** - 120-second loop with hover pause
- **Visual Effects** - Grayscale to color on hover

### 8. Awards & Recognition
- **3D Awards Carousel** - 8 award certificates
- **Auto-scroll** - Every 5 seconds with pause on interaction
- **Multiple Navigation** - Arrows, dots, keyboard, touch/swipe
- **3D Perspective** - Center focus with scaled side cards

### 9. Footer
- **Aatral Branding** - Logo and company information
- **Contact Details** - Phone, email, address
- **Quick Links** - Navigation to key sections
- **Social Links** - LinkedIn, Twitter, YouTube

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn

### Installation

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

The app will be available at `http://localhost:5173`

## 📁 Project Structure

```
safetizen-app/
├── public/
│   ├── logos/              # 31 company logos
│   ├── awards/             # 8 award certificates
│   ├── aatral-logo.png     # Aatral logo (light mode)
│   └── aatral-dark.png     # Aatral logo (dark mode)
├── src/
│   ├── App.jsx             # Main application (21+ modules data)
│   ├── index.css           # Global styles & animations
│   └── main.jsx            # Application entry point
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Pages deployment
├── index.html              # HTML template
├── package.json
├── vite.config.js          # Vite configuration
├── tailwind.config.js      # TailwindCSS configuration
└── README.md
```

## 🎨 Design Features

### Branding
- **Primary Brand**: Aatral (company)
- **Product Brand**: Safetizen™ (XR safety training platform)
- **Positioning**: Part of Aatral's Enterprise XR Training Platform Suite

### Accessibility
- **WCAG 2.1 AA Compliant** - Improved text contrast (slate-700 for light theme)
- **Keyboard Navigation** - Full support for all interactive elements
- **Screen Reader Support** - Proper ARIA labels and semantic HTML
- **Focus Indicators** - Visible on all interactive elements
- **Responsive Touch Targets** - Minimum 44px for mobile

### Responsive Design
- **Mobile First** - Optimized for 375px and up
- **Breakpoints**:
  - Mobile: < 640px (sm)
  - Tablet: 640px - 768px (md)
  - Desktop: 768px+ (lg, xl)
- **Adaptive Components**:
  - Mobile category dropdown
  - Desktop category buttons
  - Responsive navigation
  - Optimized modal layout

### Dark Mode
- **Full Support** - All components styled for dark theme
- **Automatic Detection** - Respects system preferences
- **Consistent Colors** - Proper contrast in both themes

## 🔧 Customization

### Adding/Updating Modules

Edit the `MODULES` array in `App.jsx` (starting at line 7):

```javascript
{
  name: "Module Name",
  category: "Category",
  runtime: "10 mins",
  languages: ["English", "Hindi"],
  modes: { guided: true, quiz: true, assessment: true },
  industries: ["Manufacturing", "Infrastructure"],
  devices: ["Meta Quest 3", "Meta Quest 3S"],
  description: "Module description",
  learningObjective: "What learners will achieve",
  video: "https://youtube.com/..."
}
```

### Updating Company Logos

1. Add logo images to `public/logos/`
2. Update the `logos` array in `App.jsx`:

```javascript
const logos = [
  { src: "/logos/company.jpeg", name: "Company Name" },
  // Add more logos
];
```

### Updating Awards

1. Add award images to `public/awards/`
2. Update the `awards` array in `App.jsx`:

```javascript
const awards = [
  {
    image: "/awards/award.jpg",
    title: "Award Title",
    subtitle: "Award Description"
  },
  // Add more awards
];
```

## 🌐 Deployment

### GitHub Pages (Automated)

The project includes automated deployment to GitHub Pages via GitHub Actions:

1. Push to `main` branch
2. GitHub Actions builds and deploys automatically
3. Site available at: `https://[username].github.io/SafetizenDemoSite/`

### Manual Deployment

```bash
# Build for production
npm run build

# Deploy dist/ folder to any static hosting:
# - Vercel
# - Netlify
# - AWS S3 + CloudFront
# - Any web server
```

## 🎯 Key Technologies

- **React 18** - UI framework with hooks
- **Vite** - Fast build tool and dev server
- **TailwindCSS** - Utility-first CSS framework
- **CSS Animations** - Custom keyframe animations
- **GitHub Actions** - Automated deployment

## 📱 Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🎭 Interactive Features

### Logo Carousel
- **Speed**: 120 seconds for full loop
- **Animation**: Linear infinite scroll
- **Hover**: Pauses animation
- **Effect**: Grayscale → Color transition

### Awards Carousel (3D)
- **Auto-scroll**: Every 5 seconds
- **Pause**: On hover, click, touch, or keyboard
- **Resume**: After 6 seconds of inactivity
- **3D Effect**: Center card 1.1x scale
- **Navigation**: Arrows, dots, keyboard (← →), touch/swipe

### Module Filtering
- **Real-time Search** - Instant results as you type
- **Multi-filter Support** - Combine category, language, and runtime
- **Responsive UI** - Mobile dropdown, desktop buttons
- **Smooth Transitions** - Animated filter changes

## 📊 Performance

- **Lighthouse Score**: 90+ (Performance, Accessibility, Best Practices, SEO)
- **First Contentful Paint**: < 1.5s
- **Time to Interactive**: < 3s
- **Bundle Size**: Optimized with Vite code splitting

## 📝 License

All rights reserved © Aatral

## 🤝 Contact

### Aatral
- **Website**: [aatral.io](https://aatral.io)
- **Email**: sales@aatral.io
- **Phone**: +91 7338945666 / 9830714314 / 9600067005
- **US**: +1 (669) 249-5831

### Address
Padma Vilas, Door No. 3/233, Survey No. 34/1b  
Manapakkam Main Road, Manapakkam  
Chennai - 600125, Tamil Nadu, India

---

**Built with ❤️ by Aatral** - Enterprise XR Training Solutions
