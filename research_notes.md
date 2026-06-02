# Earthfirm Sports Infra Website Plan & Prompt Guide

This document contains industry research for sports infrastructure websites, modern design trends, and custom-engineered prompts for Google AI Studio to help you build a state-of-the-art website.

---

## 1. Industry Research: Sports Infrastructure Website Structure
A sports infrastructure company needs to project high trust, precision engineering, and premium durability. Their website must present complex architectural and civil services in an easily digestible, highly visual format.

### Key Pages & Core Architecture
1. **Homepage (The Hook)**
   - **Hero Section:** Large, high-resolution imagery/video of premium courts or running tracks, bold typography, and direct Call-to-Actions (CTAs) (e.g., "Get a Quote" or "Explore Our Courts").
   - **Bento Grid Layout:** A modern grid highlighting key features (e.g., FIFA-grade turf, IAAF-approved tracks, wooden basketball courts, completed projects counter).
   - **Interactive Showcase:** A component where users can select a sport and instantly see the specific infrastructure required.
   - **Client Logos & Trust Badges:** Certifications (ISO, FIFA, IAAF, ITF) and prominent client logos.
2. **Services (The Offering)**
   - Categorized by surface/technology:
     - **Synthetic Turf:** Football fields, hockey fields, landscaping.
     - **Athletic Tracks:** Running tracks, jogging paths, PU cushions.
     - **Indoor Wooden Flooring:** Basketball courts, badminton courts, squash.
     - **Outdoor Acrylic Courts:** Tennis, basketball, volleyball courts.
     - **Lighting & Accessories:** High-mast LED stadium lighting, fencing, scoreboards.
3. **Project Portfolio (The Proof)**
   - Interactive before/after slider showing ground excavation and final court completion.
   - Filterable gallery (Filter by: Indoor, Outdoor, Turf, Wooden, Acrylic).
   - Case studies detailing size, materials used, location, and client feedback.
4. **Interactive Quote Estimator (The Lead Magnet)**
   - An interactive step-by-step wizard where the user selects:
     1. Sport Type
     2. Field/Court Dimension (Standard vs. Custom)
     3. Surface Type (Acrylic, Wood, Turf)
     4. Accessories (Fencing, Lighting)
   - Outputs a summary and collects contact details to request a callback.
5. **About Us (The Credibility)**
   - Vision, team experience, certification standards, and commitment to player safety/ergonomics.

---

## 2. Modern UI/UX Design Aesthetics
To make the website "eye-catching," "interactive," and "modern," the design should adopt the following styling standards:

- **Vibrant Accent Palettes:** Use a dark mode layout (sleek slate/black) paired with high-energy athletic accents like electric neon green, neon lime, or vibrant orange.
- **Micro-Animations:** Smooth hover effects, scroll-triggered page reveals, and fluid transitions between sections.
- **Glassmorphism:** Frosted-glass navigation bars and cards overlapping bright colorful background blurs.
- **Clean Bento Grids:** Compartmented sections with unequal dimensions that dynamically scale on mobile screens.

---

## 3. Google AI Studio Prompt Suite

Here are three specialized prompts designed to extract the best possible results from models like **Gemini 1.5 Pro** or **Gemini 2.0 Flash / 2.5 Flash** in Google AI Studio. 

> [!TIP]
> In Google AI Studio, set the **System Instructions** to:
> *"You are an elite, award-winning frontend engineer specializing in highly aesthetic, modern, and interactive single-page web applications. You use clean semantic code, modern layout concepts like Bento grids, and ensure flawless responsive behavior."*
> Set the **Temperature** to `0.2` for cleaner, syntax-error-free code generation.

### Prompt 1: Single-File Interactive Prototype (HTML + Tailwind + CSS + JS)
Use this prompt to generate a complete, working website mockup in a single file that you can save as `.html` and run instantly in any browser.

```text
Build a highly aesthetic, modern, responsive, and interactive single-page website for "Earthfirm Sports Infra", a premium sports infrastructure construction company.

Technology Stack:
- Core structure: HTML5 with semantic tags.
- Styling: Tailwind CSS (via CDN) supplemented by custom embedded CSS in <style> tags.
- Icons: Lucide Icons or FontAwesome (via CDN).
- Typography: Import Outfit or Inter font from Google Fonts.
- JavaScript: Vanilla JS for interactive features and state management.

Design Guidelines:
- Color Palette: Sleek Dark Mode. Deep charcoal/slate background (#0B0F19), card backgrounds (#161D30), with vibrant energetic accents of Neon Sports Green (#39FF14 or #10B981) and Electric Orange (#FF5733).
- Layout: Modern Bento-grid for the services section, glassy navigation bar with blur, and big bold headings.
- Animations: Smooth hover transitions, fade-in active states, and a fluid mobile menu toggler.

Sections to Include:
1. Nav Bar: Glassmorphism style, sticky top, with links (Home, Services, Gallery, Estimator, Contact) and a "Get a Quote" CTA button. Responsive hamburger menu for mobile.
2. Hero Section: Bold, oversized typography ("WE BUILD THE STAGES WHERE LEGENDS ARE MADE"). High-contrast dark sports court background graphic (using clean SVG overlays or Unsplash sports images). Split layout: left text and CTA buttons, right an interactive preview showing key metrics (e.g., 500+ Courts Built, 10+ Years Exp).
3. Core Services (Bento Grid): A beautiful layout of uneven grids. Clicking a grid card expands details or shows a popup about that service (Synthetic Turf, Athletic Tracks, Indoor Wood Flooring, Acrylic Courts).
4. Interactive Sports Court Customizer (The Interactive Hook): An SVG-based interactive mini-court visualizer. The user can click buttons to switch between a Tennis Court, Basketball Court, and Badminton Court. They can also change the court colors (e.g., Classic Blue, Forest Green, Brick Red) and the line colors. The SVG court colors should dynamically update via JavaScript.
5. Interactive Quote Estimator: A clean multi-step calculator form where visitors select court type, dimensions, and optional accessories. It calculates a mock estimation score and offers a form to "Submit details for a final quote".
6. Footer: Clean links, contact info, and ISO/FIFA compliance statements.

Deliver clean, fully commented, single-file HTML code containing all styles and scripts. Make sure the UI looks incredibly premium and is optimized for both desktop and mobile.
```

### Prompt 2: Modern React Component Code (Tailwind + Lucide)
Use this prompt if you are building the website using React/Next.js and want to generate reusable components.

```text
Act as an expert React developer. Write a modern React component for a sports infrastructure company homepage named "Earthfirm Sports Infra".

Requirements:
- Use React hooks (useState, useEffect) for managing interactive states.
- Style the component using Tailwind CSS utility classes.
- Use 'lucide-react' for all icons.
- Implement an interactive tennis/basketball court customizer inside the UI where the user can click colors to update an SVG court visualization.
- Implement a step-by-step interactive quote estimator with a progress bar.
- Make the layout clean, utilizing a dark bento-grid theme with neon green accents.
- Provide clean, production-ready code with typescript definitions (or clean Javascript if preferred, please specify typescript).
```

### Prompt 3: Sports Court Interactive Visualizer Widget
Use this prompt if you want to focus heavily on the interactive visualizer and build it as a standout widget.

```text
Develop a lightweight, highly interactive Sports Court Color & Type Visualizer widget using HTML, CSS, and vanilla JS (or React).

Visualizer Details:
- Display a clean SVG drawing of a sports court (with court boundary lines, key, center circle, net/hoops).
- Provide UI toggle buttons to switch the court layout between:
  1. Tennis Court
  2. Basketball Court
  3. Futsal/Multipurpose Court
- Provide a color palette selector (e.g., Forest Green, Royal Blue, Terracotta Red, Ocean Teal) for the inner court area, outer court area, and line markings.
- Clicking any color swatch must instantly transition the SVG fill/stroke colors using CSS transitions.
- Make the design sleek, compact, and ready to be embedded as an iframe or direct block on a website homepage.
```
