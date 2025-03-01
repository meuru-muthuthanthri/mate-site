# Mate Sri Lanka - IT Services Website

A professional website for Mate Sri Lanka, a company providing IT services to Sri Lankan businesses.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Hosting on GitHub Pages](#hosting-on-github-pages)
- [Customization](#customization)
- [License](#license)

## Overview

This is a responsive, modern website for Mate Sri Lanka IT Services. The website showcases the company's services, portfolio, testimonials, and contact information. It is designed to be professional, user-friendly, and optimized for all devices.

## Features

- Responsive design that works on all devices
- Modern and professional UI/UX
- Interactive elements with smooth animations
- Contact form for client inquiries
- Newsletter subscription
- Testimonial slider
- Service showcase
- Portfolio gallery
- About section with company statistics

## Project Structure

```
mate-sri-lanka/
├── index.html              # Main HTML file
├── css/
│   └── styles.css          # CSS styles
├── js/
│   └── script.js           # JavaScript functionality
├── images/                 # Image assets (to be added)
└── README.md               # Project documentation
```

## Getting Started

To run this website locally:

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/mate-sri-lanka.git
   ```

2. Navigate to the project directory:
   ```
   cd mate-sri-lanka
   ```

3. Open `index.html` in your browser.

## Hosting on GitHub Pages

Follow these steps to host your website on GitHub Pages:

### 1. Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in to your account.
2. Click on the "+" icon in the top right corner and select "New repository".
3. Name your repository (e.g., "mate-sri-lanka").
4. Choose "Public" visibility.
5. Click "Create repository".

### 2. Upload Your Website Files

#### Option 1: Using Git Command Line

1. Initialize Git in your project folder:
   ```
   git init
   ```

2. Add all files to Git:
   ```
   git add .
   ```

3. Commit the files:
   ```
   git commit -m "Initial commit"
   ```

4. Add the remote repository:
   ```
   git remote add origin https://github.com/yourusername/mate-sri-lanka.git
   ```

5. Push to GitHub:
   ```
   git push -u origin main
   ```

#### Option 2: Using GitHub Web Interface

1. In your new repository, click on "uploading an existing file".
2. Drag and drop all your website files and folders.
3. Click "Commit changes".

### 3. Configure GitHub Pages

1. Go to your repository on GitHub.
2. Click on "Settings" tab.
3. Scroll down to the "GitHub Pages" section.
4. Under "Source", select "main" branch.
5. Click "Save".
6. Wait a few minutes for GitHub to build your site.
7. Your site will be published at `https://yourusername.github.io/mate-sri-lanka/`.

### 4. Add a Custom Domain (Optional)

1. Purchase a domain name from a domain registrar (e.g., Namecheap, GoDaddy).
2. In your repository settings, under "GitHub Pages", enter your custom domain in the "Custom domain" field.
3. Click "Save".
4. Configure your domain's DNS settings:
   - Add an `A` record pointing to GitHub Pages IP addresses:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - Or add a `CNAME` record pointing to `yourusername.github.io`.
5. Wait for DNS changes to propagate (can take up to 48 hours).

## Customization

### Images

Replace the placeholder images with your own:

1. Add your images to the `images/` directory.
2. Update the image paths in `index.html`.

### Content

1. Edit the text in `index.html` to match your business information.
2. Update service descriptions, portfolio items, and testimonials.
3. Change contact information and social media links.

### Styling

1. Modify colors and styles in `css/styles.css`.
2. The website uses CSS variables for colors, making it easy to change the color scheme:
   ```css
   :root {
       --primary-color: #2563eb;
       --secondary-color: #1e40af;
       /* other color variables */
   }
   ```

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---

© 2023 Mate Sri Lanka. All Rights Reserved. 