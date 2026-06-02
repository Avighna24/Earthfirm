# Google AI Studio Prompts for Earthfirm Sports Infra

Below are ready-to-use prompts you can copy and paste into Google AI Studio (e.g., using **Gemini 1.5 Pro**, **Gemini 2.0 Flash**, or **Gemini 2.5 Pro**) to continue building or upgrading your website.

---

### Option A: Prompt to Refine/Modify the Current HTML Prototype
Use this prompt if you want to update the existing `index.html` file with your official logo, custom colors, or updated contact details.

> [!IMPORTANT]
> **How to use:** Paste the contents of your `index.html` file into Google AI Studio, and then append the prompt below.

```text
I have a single-file HTML prototype for my sports infrastructure company, "Earthfirm Sports Infra" (attached/pasted above). 

Please modify this HTML file to incorporate my new brand assets:
1. Brand Logo: [Insert logo description, text, or SVG code here]
2. Brand Color Palette:
   - Primary Accent: [Insert Hex Code, e.g., #00F3FF]
   - Secondary Accent: [Insert Hex Code]
   - Base Backgrounds: [Insert Hex Code]
3. Custom Updates:
   - [Add any wording changes, e.g., "Change the phone number to +91 99999 99999"]
   - [Add any court adjustments, e.g., "Add Pickleball as a separate layout in the SVG customizer"]

Deliver the complete updated single-file HTML code with Tailwind CSS and JS intact. Ensure the dark bento-grid aesthetic and smooth micro-interactions remain fully functional.
```

---

### Option B: Prompt to Port the HTML Prototype to React (Next.js / Vite)
Use this prompt when you are ready to upgrade from the single-file HTML prototype to a modern React frontend.

> [!IMPORTANT]
> **How to use:** Upload your `index.html` to Google AI Studio and run this prompt.

```text
Act as an expert React developer. I have an interactive HTML prototype for "Earthfirm Sports Infra" (attached above). Port this entire prototype into a modern React application.

Requirements:
1. Framework: [Specify Vite + React OR Next.js App Router].
2. Styling: Use Tailwind CSS with clean utility classes.
3. Component Structure: Break the single page down into reusable components:
   - Header/Navbar (with stateful mobile drawer)
   - HeroSection
   - SportsBentoGrid (with interactive details modal)
   - CourtCustomizer (with stateful SVG rendering)
   - QuoteEstimator (stateful multi-step form wizard)
   - GallerySection (with the before/after slider component)
   - Footer
4. Icons: Convert all icon references to use the 'lucide-react' library.
5. Code Quality: Provide clean, production-ready TypeScript code with proper type definitions for the court customizer states and project estimator calculator.
```

---

### Option C: Prompt to Build a Node.js Backend for Form Submissions
Use this prompt if you want Google AI Studio to write a backend server (Node.js/Express) to receive and store the inquiries submitted via the Quote Estimator.

```text
Write a clean, secure Node.js and Express backend server to handle form submissions from the "Earthfirm Sports Infra" Quote Estimator wizard.

The server should:
1. Expose a POST endpoint `/api/quote-requests` that accepts:
   - clientName (string)
   - clientEmail (string)
   - selectedSport (string)
   - sizeCategory (string)
   - subBaseType (string)
   - upgrades (array of strings, e.g., ['lighting', 'fencing'])
   - estimatedCost (number)
   - estimatedDuration (string)
2. Validate incoming requests using a schema validator (like Joi or Zod).
3. Database: Save the request details to a [Specify database: MongoDB/PostgreSQL/SQLite] database.
4. Notifications: Integrate a mailer library (like Nodemailer or Resend) to send a confirmation email containing the PDF-style quote proposal summary to the client, and a notification email to the Earthfirm sales team.

Provide the complete server code, database connection setup, and setup instructions.
```
