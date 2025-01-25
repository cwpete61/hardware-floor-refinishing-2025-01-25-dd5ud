# Tykoon Wood Floors Landing Page - Maintenance Guide

This guide will help you maintain and customize the Tykoon Wood Floors landing page. Whether you're new to web development or just getting started, follow these instructions to make updates safely and effectively.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your company name and navigation menu. To update:

1. Company Name:
```html
<!-- Find this line in the header -->
<div class="text-2xl font-bold text-gray-800">Tykoon Wood Floors</div>
```
Simply replace "Tykoon Wood Floors" with your company name.

### Hero Section
Located at the top of the page with the main headline:

1. Update Main Headline:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight mb-8">
    Hardware Floor Refinishing
</h1>
```
Replace "Hardware Floor Refinishing" with your desired headline.

2. Update Subheading:
```html
<p class="text-xl md:text-2xl text-gray-600 leading-relaxed mb-12">
    Transform Your Home with Tykoon Wood Floors...
</p>
```

### Understanding Tailwind Classes
Common classes used in this template:

- Text sizes: `text-xl`, `text-2xl`, `text-3xl`, etc.
- Colors: `text-gray-800`, `bg-blue-600`, etc.
- Spacing: `px-4` (padding left/right), `py-4` (padding top/bottom), `mb-8` (margin bottom)
- Responsive prefixes: `md:` (medium screens), `lg:` (large screens)

Example of modifying a button:
```html
<!-- Original -->
<a href="https://site.com" class="inline-block bg-blue-600 text-white text-lg px-8 py-4 rounded-full">

<!-- To change color to green -->
<a href="https://site.com" class="inline-block bg-green-600 text-white text-lg px-8 py-4 rounded-full">
```

## Managing Links

### Navigation Menu Links
The navigation menu contains internal links to page sections:

```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

To update:
1. Internal links (starting with #) connect to section IDs
2. External links need full URLs
3. Replace "https://site.com" with your actual website URL

### Call-to-Action Buttons
Located in hero and CTA sections:

```html
<!-- Find and update these URLs -->
<a href="https://site.com" class="inline-block bg-blue-600...">Schedule a Consultation</a>
```

## Adding Privacy and Terms Pages

### Step 1: Create New Pages
Create two new files in your website directory:
- privacy.html
- terms.html

### Step 2: Update Footer Links
Locate this section in the footer:
```html
<div>
    <h4 class="text-lg font-semibold text-white mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues

1. Broken Internal Links
- Ensure section IDs match navigation links
- Example: `href="#features"` needs matching `id="features"` in section tag

2. Responsive Design Issues
- Don't remove `md:` or `lg:` prefixes from classes
- Keep the viewport meta tag in header:
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

3. Font Awesome Icons Not Showing
- Verify the Font Awesome CDN link is present in header
- Check icon class names match Font Awesome 6 naming

### Getting Help
- Inspect elements using browser developer tools (Right-click > Inspect)
- Verify all files are in the correct directory
- Double-check all closing tags match opening tags
- Ensure Tailwind CSS CDN link remains in the header

Remember to always backup your files before making changes, and test on multiple devices and browsers after updates.

For additional help or specific customization needs, consult the [Tailwind CSS documentation](https://tailwindcss.com/docs) or reach out to your web development team.