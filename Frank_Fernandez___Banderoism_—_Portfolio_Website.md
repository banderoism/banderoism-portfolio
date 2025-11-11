# Frank Fernandez | Banderoism — Portfolio Website

A clean, professional one-page portfolio website for Frank Fernandez, a Video Producer & Editor operating under the creative identity Banderoism.

## Features

✅ **Responsive Design** — Mobile-first layout that works on all devices
✅ **Hero Section** — Eye-catching headline with call-to-action
✅ **Embedded Reel** — YouTube/Vimeo video showcase
✅ **Portfolio Grid** — 6 projects organized by category (Commercial, Event, Aerial)
✅ **Modal Functionality** — Click to view project details with video embeds
✅ **Services Section** — Three service offerings with pricing
✅ **Contact Form** — Integrated with Formspree for email submissions
✅ **Social Links** — Instagram and YouTube integration
✅ **SEO Optimized** — Meta tags, structured content, and semantic HTML
✅ **Smooth Navigation** — Anchor links with smooth scrolling

## Design System

- **Fonts:** Raleway (headlines), Montserrat (body)
- **Colors:** White background, Charcoal text (#2c2c2c), Muted Olive accent (#6B705C)
- **Layout:** Spacious, clean, professional
- **Breakpoints:** Mobile (480px), Tablet (768px), Desktop (1200px+)

## File Structure

```
banderoism-portfolio/
├── index.html          # Main HTML file with all sections
├── css/
│   └── styles.css      # Complete styling and responsive design
├── js/
│   └── script.js       # Modal functionality and interactivity
├── images/             # Directory for custom images
└── README.md           # This file
```

## Setup Instructions

### Local Development

1. **Clone or download the project**
   ```bash
   cd banderoism-portfolio
   ```

2. **Start a local server**
   ```bash
   # Using Python 3
   python3 -m http.server 8000
   
   # Or using Node.js
   npx http-server
   ```

3. **Open in browser**
   - Navigate to `http://localhost:8000`

### Customization

#### Update Contact Form
The contact form is configured to use Formspree. To enable email submissions:

1. Go to [formspree.io](https://formspree.io)
2. Create a new form and get your Form ID
3. In `index.html`, update the form action:
   ```html
   <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

#### Update Email Address
Replace `frank@banderoism.com` with the actual email address in the Contact section.

#### Update Social Links
Update the social media URLs in the Contact section:
```html
<a href="https://instagram.com/your-handle" target="_blank">Instagram</a>
<a href="https://youtube.com/@your-channel" target="_blank">YouTube</a>
```

#### Add Portfolio Projects
Replace placeholder videos and images:
1. Update YouTube embed URLs in the modals
2. Replace placeholder images with actual project thumbnails
3. Update project titles, roles, deliverables, and results

## Deployment Options

### Netlify
1. Push your code to GitHub
2. Connect your repository to Netlify
3. Deploy with one click

### Vercel
1. Push your code to GitHub
2. Import project in Vercel
3. Deploy automatically

### Replit
1. Create a new Replit project
2. Upload the files
3. Run and share the live link

### Traditional Hosting
1. Upload files to your web server via FTP
2. Ensure `.html`, `.css`, and `.js` files are in the correct directories
3. Access via your domain

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance Optimization

- Lazy-loaded video embeds for faster page load
- Optimized CSS with minimal file size
- Vanilla JavaScript (no dependencies)
- Responsive images with proper sizing

## SEO Features

- Meta description and keywords
- Semantic HTML structure
- Proper heading hierarchy
- Alt text for images
- Open Graph meta tags ready for customization

## Future Enhancements

- Add real portfolio images and videos
- Implement analytics tracking
- Add blog section
- Integrate email newsletter signup
- Add testimonials section
- Implement dark mode toggle

## Support

For questions or issues, contact Frank Fernandez directly or refer to the contact form on the website.

---

**Built with:** HTML5, CSS3, Vanilla JavaScript
**Last Updated:** November 2025
