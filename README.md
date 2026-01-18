# Modern Portfolio Website

A clean, modern, and responsive portfolio website built with HTML, CSS, and JavaScript. Perfect for developers, designers, and freelancers to showcase their work and skills.

![Portfolio Preview](https://via.placeholder.com/800x400/667eea/ffffff?text=Portfolio+Preview)

## 🚀 Features

- **Responsive Design** - Works perfectly on desktop, tablet, and mobile devices
- **Modern UI/UX** - Clean and minimal design with smooth animations
- **Interactive Elements** - Hover effects, smooth scrolling, and dynamic content
- **Project Filtering** - Filter projects by category (Web Apps, Mobile, API, UI/UX)
- **Contact Form** - Functional contact form with validation
- **SEO Optimized** - Proper meta tags and semantic HTML structure
- **Performance Optimized** - Fast loading times and smooth animations
- **Accessibility** - WCAG compliant with proper ARIA labels and keyboard navigation

## 📁 Project Structure

```
portfolio/
├── index.html              # Homepage
├── about.html              # About Me page
├── projects.html           # Projects showcase
├── contact.html            # Contact page
├── css/
│   ├── style.css           # Main stylesheet
│   ├── responsive.css      # Mobile responsive styles
│   └── components.css      # Reusable components (if needed)
├── js/
│   ├── main.js             # Core JavaScript functionality
│   ├── navigation.js       # Navigation and mobile menu
│   ├── animations.js       # Scroll animations and effects
│   ├── projects-filter.js  # Project filtering functionality
│   └── contact-form.js     # Contact form validation and submission
├── images/
│   ├── profile.jpg         # Your professional photo
│   ├── about-photo.jpg     # About page image
│   └── projects/           # Project screenshots
│       ├── ecommerce-platform.jpg
│       ├── task-manager.jpg
│       ├── weather-app.jpg
│       ├── rest-api.jpg
│       ├── portfolio-design.jpg
│       └── blog-cms.jpg
├── assets/
│   ├── cv.pdf              # Your resume/CV for download
│   └── fonts/              # Custom fonts (if needed)
└── README.md               # This file
```

## 🛠️ Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- A code editor (VS Code, Sublime Text, etc.)
- Basic knowledge of HTML, CSS, and JavaScript

### Installation

1. **Clone or Download the Portfolio**
   ```bash
   git clone https://github.com/yourusername/portfolio.git
   # or download and extract the ZIP file
   ```

2. **Navigate to the Project Directory**
   ```bash
   cd portfolio
   ```

3. **Customize the Content**
   - Open `index.html` and replace "John Doe" with your name
   - Update personal information in all HTML files
   - Replace placeholder images with your actual photos and project screenshots
   - Update social media links, email, and contact information

4. **Test the Website**
   - Open `index.html` in your web browser
   - Test on different devices and screen sizes
   - Check all links and functionality

### Customization Guide

#### 1. Personal Information

**Update your name and title:**
```html
<!-- In all HTML files -->
<title>Your Name - Your Title</title>
<!-- and -->
<h1>Hello, I'm <span class="highlight">Your Name</span></h1>
<h2>Your Professional Title</h2>
```

**Update contact information:**
```html
<!-- In contact.html -->
<p>john.doe@email.com</p>
<p>+1 (555) 123-4567</p>
<p>Your City, Country</p>
```

#### 2. Social Media Links

**Update social media URLs:**
```html
<!-- In all HTML files -->
<a href="https://github.com/yourusername" target="_blank">
<a href="https://linkedin.com/in/yourusername" target="_blank">
<a href="https://twitter.com/yourusername" target="_blank">
<a href="https://instagram.com/yourusername" target="_blank">
```

#### 3. Profile Photo

**Replace profile image:**
- Add your professional photo to the `images/` folder
- Name it `profile.jpg` (or update the HTML to match your filename)
- Recommended size: 400x400 pixels
- Format: JPG or PNG

#### 4. Projects

**Update project information:**
```html
<!-- In projects.html -->
<h3 class="project-title">Your Project Name</h3>
<p class="project-description">Your project description</p>
<div class="project-tech">
    <span class="tech-tag">Technology 1</span>
    <span class="tech-tag">Technology 2</span>
</div>
```

**Add project screenshots:**
- Add project images to `images/projects/` folder
- Recommended size: 600x400 pixels
- Update the `src` attribute in the HTML

#### 5. Skills and Experience

**Update skills in about.html:**
```html
<!-- Update skill percentages -->
<div class="skill-progress" data-progress="95"></div>
```

**Update experience timeline:**
```html
<!-- In about.html timeline section -->
<span class="timeline-date">2024 - Present</span>
<h3>Your Job Title</h3>
<p>Your Company</p>
<p>Your job description</p>
```

#### 6. Resume/CV

**Add your resume:**
- Place your PDF resume in the `assets/` folder
- Name it `cv.pdf`
- Update the download link in `index.html`

## 🎨 Customization Options

### Colors

The main color scheme uses a gradient from #667eea to #764ba2. To change colors:

```css
/* In style.css - look for these variables */
.highlight {
    background: linear-gradient(135deg, #your-color-1 0%, #your-color-2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.btn-primary {
    background: linear-gradient(135deg, #your-color-1 0%, #your-color-2 100%);
}
```

### Typography

The portfolio uses the Inter font family from Google Fonts. To change:

```html
<!-- In the <head> section of all HTML files -->
<link href="https://fonts.googleapis.com/css2?family=YourFont:wght@300;400;500;600;700&display=swap" rel="stylesheet">
```

Then update the CSS:
```css
/* In style.css */
body {
    font-family: 'YourFont', sans-serif;
}
```

### Layout

The portfolio uses CSS Grid and Flexbox for responsive layouts. Modify breakpoints in `responsive.css`:

```css
/* In responsive.css */
@media screen and (max-width: 1024px) { /* Tablet styles */ }
@media screen and (max-width: 768px) { /* Mobile styles */ }
@media screen and (max-width: 480px) { /* Small mobile styles */ }
```

## 📱 Browser Support

- Chrome 60+
- Firefox 60+
- Safari 12+
- Edge 79+
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🔧 Advanced Features

### Adding Google Analytics

1. Create a Google Analytics account
2. Add your tracking code to all HTML files before the closing `</head>` tag:

```html
<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_TRACKING_ID');
</script>
```

### Adding a Blog

To add a blog section:
1. Create a `blog.html` page
2. Add blog posts as separate HTML files or use a static site generator
3. Update the navigation menu to include the blog link

### Contact Form Backend

The contact form currently shows a success message. To make it functional:

1. **Using Formspree (Recommended):**
   - Sign up at [formspree.io](https://formspree.io)
   - Replace the form action with your Formspree endpoint

2. **Using Netlify Forms:**
   - Add `netlify` attribute to the form tag
   - Deploy to Netlify

3. **Custom Backend:**
   - Create a server-side script (PHP, Node.js, Python, etc.)
   - Update the form action to point to your endpoint

## 🚀 Deployment

### GitHub Pages

1. Push your code to a GitHub repository
2. Go to Settings > Pages
3. Select source branch (usually `main` or `master`)
4. Your site will be available at `https://yourusername.github.io/repository-name`

### Netlify

1. Connect your GitHub repository to Netlify
2. Set build command: (leave empty for static sites)
3. Set publish directory: `/`
4. Deploy automatically on every push

### Vercel

1. Import your GitHub repository to Vercel
2. Configure build settings (usually automatic for static sites)
3. Deploy with custom domain support

### Traditional Web Hosting

1. Upload all files to your web server's public directory
2. Ensure the file structure is maintained
3. Access via your domain

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Feel free to fork this project and customize it for your own use. If you make improvements that could benefit others, pull requests are welcome!

## 📞 Support

If you need help customizing this portfolio:

1. Check the documentation above
2. Review the code comments for detailed explanations
3. Feel free to open an issue for questions or bug reports

## 🎯 Performance Tips

1. **Optimize Images:**
   - Use WebP format when possible
   - Compress images without losing quality
   - Use appropriate image sizes for different screen densities

2. **Minimize Files:**
   - Minify CSS and JavaScript for production
   - Use a CDN for external libraries

3. **Caching:**
   - Enable browser caching for static assets
   - Consider using a service worker for offline functionality

## 🔍 SEO Optimization

The portfolio is already optimized for SEO, but you can enhance it further:

1. **Update Meta Tags:**
   ```html
   <meta name="description" content="Your custom description">
   <meta name="keywords" content="your, keywords, here">
   <meta property="og:title" content="Your Name - Portfolio">
   <meta property="og:description" content="Your description">
   <meta property="og:image" content="images/og-image.jpg">
   ```

2. **Add Structured Data:**
   ```html
   <script type="application/ld+json">
   {
     "@context": "https://schema.org",
     "@type": "Person",
     "name": "Your Name",
     "jobTitle": "Your Title",
     "url": "https://yourwebsite.com"
   }
   </script>
   ```

---

**Happy coding! 🎉**

If you use this portfolio template, please give it a star ⭐ and share it with others!