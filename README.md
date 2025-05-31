# Triveni-webapp

## Purpose
A simple, static web app to replace Triveni Supermarket’s large WhatsApp group:
- Show announcements in a clean, chat‐style feed
- Provide one‐tap “Message on WhatsApp” and “Call Store” buttons
- Include an embedded “Contact Us” form so customers can send messages directly

## Core Features
- **Landing Page (index.html):**  
  • “Welcome to Triveni Supermarket Updates!” heading  
  • Two buttons: WhatsApp chat + Phone call  
- **Announcements Page (announcements.html):**  
  • Fetches and displays announcements from `announcements.json`  
  • Shows each announcement as a “bubble” (with optional image)  
  - Error banner if JSON fails to load  
  - Quick‐action buttons below the feed  
- **Contact Page (contact.html):**  
  • Embedded Google Form (or Formspree) for Name / Email / Message  
  - Quick‐action buttons below the form  

## How to Update Content
1. **Announcements:**  
   - Edit `announcements.json` to add, remove, or modify announcements.  
   - Commit & push—Netlify/Vercel will auto‐redeploy.  
2. **Contact Form:**  
   - In Google Forms (or Formspree), generate a new embed `<iframe>` or form snippet.  
   - Paste it into `contact.html`.  
   - Commit & push—site auto‐redeploys.

## One‐Time Setup Instructions
1. **Clone** this repo:  
   ```bash
   git clone https://github.com/ukkandi/Triveni-webapp.git
   cd triveni-app
