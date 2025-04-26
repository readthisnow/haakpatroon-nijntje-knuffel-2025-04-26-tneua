# Landing Page Maintenance Guide

This guide will help you maintain and customize your Nijntje landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common maintenance tasks.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Main Sections to Update

#### Header Text
```html
<!-- Located in the navigation section -->
<a href="#" class="text-2xl font-bold text-indigo-600">Nijntje</a>
```
To change the logo text, simply replace "Nijntje" with your desired text.

#### Hero Section
```html
<h1 class="text-4xl sm:text-5xl lg:text-6xl font-bold text-gray-900 mb-6 leading-tight">
    Haakpatroon Nijntje Knuffel
</h1>
<p class="text-xl sm:text-2xl text-gray-600 mb-8">
    Koop Haakpatroon Nijntje Knuffel Met Korting
</p>
```
To modify:
1. Replace the h1 text between the tags
2. Update the subtitle in the paragraph tag
3. Keep the classes intact to maintain styling

### Understanding Tailwind Classes

Key classes explained:
- `text-4xl`: Large text size (mobile)
- `sm:text-5xl`: Larger text on small screens
- `lg:text-6xl`: Largest text on large screens
- `mb-6`: Margin bottom spacing
- `text-gray-900`: Dark gray text color

### Modifying Responsive Design

Example of responsive class structure:
```html
<div class="text-base md:text-lg lg:text-xl">
```
- Base size: `text-base`
- Medium screens: `md:text-lg`
- Large screens: `lg:text-xl`

## Fixing Broken Links

### Navigation Menu Links
Current navigation links:
```html
<div class="hidden lg:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Voordelen</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

To update:
1. Locate the `href` attribute
2. Replace the "#section-name" with:
   - Internal links: `#new-section-id`
   - External links: `https://full-url.com`

### Call-to-Action Links
```html
<a href="https://amzn.to/4jPt4Xc" class="inline-block bg-indigo-600...">
    Bekijk Aanbieding
</a>
```
Replace `https://amzn.to/4jPt4Xc` with your new URL.

## Linking Privacy and Terms Pages

### Adding Footer Links
Locate the footer section:
```html
<footer class="bg-gray-900 text-gray-300 py-12">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
        <!-- Add the following code -->
        <div class="mt-4 space-x-4">
            <a href="/privacy.html" class="hover:text-white transition-colors duration-300">
                Privacy Policy
            </a>
            <a href="/terms.html" class="hover:text-white transition-colors duration-300">
                Terms of Service
            </a>
        </div>
    </div>
</footer>
```

### Style Consistency
Use these classes for new links to match existing styling:
```html
class="text-gray-300 hover:text-white transition-colors duration-300"
```

## Troubleshooting

### Common Issues

1. **Broken Layout**
   - Check for missing closing tags
   - Verify Tailwind CSS classes are spelled correctly
   - Ensure responsive classes use correct breakpoints (sm:, md:, lg:)

2. **Links Not Working**
   - Verify file paths are correct
   - Check if section IDs match href attributes
   - Ensure external URLs include "https://"

3. **Responsive Issues**
   - Test on different screen sizes
   - Verify mobile menu functionality
   - Check responsive classes are properly ordered

### Best Practices

1. Always backup before making changes
2. Test changes in a development environment first
3. Validate HTML using W3C validator
4. Test all links after updating
5. Check mobile responsiveness using browser dev tools

Need help? Contact technical support at [support email].

---

This guide specifically addresses the structure and elements of your Nijntje landing page. For additional customization needs or technical support, please refer to the Tailwind CSS documentation or consult with your web development team.