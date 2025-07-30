# Digital Business Card Project

This is a simple, clean, and responsive **digital business card** built using **HTML**, **CSS**, **Flexbox**, and a touch of **JavaScript**. The goal is to visually present personal or professional details in a modern, card‑style layout — perfect for a portfolio, personal site, or small business — with an easy one‑click “Download vCard” feature for quick mobile import.

## Features

* Responsive layout using **CSS Flexbox**  
* Clean and minimal design  
* Profile picture and name display  
* Role/title and short bio or description  
* **Download vCard** button that auto‑triggers a `.vcf` download (or direct Contacts import on mobile)  
* Easily customizable for personal use  

## Technologies Used

* **HTML5** – structure and content  
* **CSS3** – styling and layout  
* **Flexbox** – for modern and responsive alignment  
* **JavaScript (ES6)** – to wire up the Download vCard button  
* (Optional) **Google Fonts** – for better typography  

## Live Demo

You can view the live, publicly hosted version of this project at:  
**[estanler-aleman-businesscard.netlify.app](https://estanler-aleman-businesscard.netlify.app)**

## File Structure

```
project-folder/
│
├── index.html # Main HTML file with .card-box and vCard button
├── styles.css # CSS file for styling the card
├── script.js # JavaScript to handle auto‑triggering the vCard download
├── EstanlerAleman.vcf # Pre‑generated vCard file for one-click import
└── /Images/ # Folder to store profile picture or assets
└── Estanler headshot.JPG
```


## How It Works

1. **HTML**  
   - A hidden `<a href="EstanlerAleman.vcf" download>` tag sits next to a visible `<button>` with id `download-vcard-btn`.  
2. **CSS**  
   - Flexbox handles layout of the card and positions the button beneath it.  
   - Button styles (including hover effects) are defined in `styles.css`.  
3. **JavaScript** (`script.js`)  
   - Listens for clicks on the “Download My vCard” button.  
   - Programmatically “clicks” the hidden link, starting the `.vcf` download.  
   - On mobile browsers, this opens the Contacts import flow immediately.  

## Customization Tips

* Replace the profile picture in `/Images/` with your own.  
* Swap out the vCard contents in `EstanlerAleman.vcf` for your personal info.  
* Tweak button colors and hover states in `styles.css`.  
* Extend `script.js` with other interactions (theme toggles, copy‑to‑clipboard, etc.).  

## Future Ideas

* Add a **dark / light mode** toggle via JavaScript and CSS custom properties.  
* Implement a **Copy Email** or **Copy Phone** snippet using the Clipboard API.  
* Fade‑in animations on scroll with an Intersection Observer.  
* Embed a QR code that encodes the vCard for quick scanning.  
* Hook up a live contact form that sends messages via AJAX.  

---

### Final Notes

This project demonstrates a modern, web‑friendly digital business card that combines solid layout fundamentals with a small JavaScript enhancement to streamline contact import—especially on mobile devices. Feel free to fork, customize, and build upon it for your own personal brand or client work!  

