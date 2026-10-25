# GEMINI.md

## Project Overview
This is a professional portfolio website for **Kushal Bhatia**, a Senior Associate Consultant and Full Stack Developer. The project is a static web application built using traditional web technologies and modern CSS preprocessors.

### Core Technologies
- **Frontend:** HTML5, Vanilla JavaScript, jQuery.
- **Styling:** SCSS (SASS), Bootstrap 4.
- **Hosting & Deployment:** Firebase Hosting.
- **Interactions & Animations:** 
  - [AOS](https://michalsnik.github.io/aos/) (Animate On Scroll)
  - [Owl Carousel](https://owlcarousel2.github.io/OwlCarousel2/)
  - [Magnific Popup](https://dimsemenov.com/plugins/magnific-popup/)
  - [Stellar.js](http://markdalgleish.com/projects/stellar.js/) (Parallax)
  - [Waypoints](http://imakewebthings.com/waypoints/)
- **Services:**
  - [EmailJS](https://www.emailjs.com/) for contact form submissions.

## Directory Structure
- `index.html`: Main landing page containing all portfolio sections (About, Resume, Services, Projects, Contact).
- `single.html`: Secondary page template.
- `scss/`: Source SASS files, including a customized Bootstrap integration.
- `css/`: Compiled CSS files (main entry point: `style.css`).
- `js/`: JavaScript logic (main entry point: `main.js`).
- `images/`: Static assets including project screenshots and background images.
- `fonts/`: Icon fonts and web fonts.
- `alertJS/`: Custom internal library for alert notifications.

## Building and Running

### Local Development
This project uses **Prepros** for local development, SCSS compilation, and live reloading.
- **SCSS Compilation:** Prepros watches the `scss/` directory and compiles `style.scss` into `css/style.css`.
- **Local Server:** Prepros provides a local server (typically on port 8026 as per `prepros-6.config`).
- **Manual Run:** Since it's a static site, you can also simply open `index.html` in any web browser.

### Deployment
The project is configured for **Firebase Hosting**.
- **Prerequisites:** Firebase CLI installed (`npm install -g firebase-tools`).
- **Command:** 
  ```bash
  firebase deploy
  ```
- **Configuration:** Defined in `firebase.json` and `.firebaserc`.

## Development Conventions
- **Styles:** Modify styles in the `scss/` directory rather than directly editing `css/style.css`.
- **Interactivity:** Most UI logic is handled in `js/main.js` using jQuery and various plugins.
- **Contact Form:** The contact form integration uses EmailJS; the initialization and submission logic are embedded in `index.html` and `js/main.js`.
- **Responsive Design:** Follows Bootstrap 4 grid conventions.
