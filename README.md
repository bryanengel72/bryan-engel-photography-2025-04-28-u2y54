# Bryan Engel Photography Landing Page - Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the Bryan Engel Photography landing page. Whether you're new to web development or need a quick reference, follow these step-by-step instructions.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<!-- Located at the top of the page -->
<div class="text-2xl font-bold">
    <a href="#" class="text-gray-800 hover:text-gray-600 transition-colors duration-300">Bryan Engel</a>
</div>
```
To update the business name:
1. Locate this section in the code
2. Replace "Bryan Engel" with your desired text
3. Keep the surrounding HTML tags intact

#### Hero Section
```html
<div class="max-w-4xl mx-auto text-center text-white">
    <h1 class="text-4xl md:text-6xl font-bold mb-6 leading-tight">Bryan Engel Photography</h1>
    <p class="text-xl md:text-2xl mb-8">Taking your photography to the next level</p>
</div>
```
To modify:
1. Update the h1 text for your main headline
2. Change the paragraph text for your tagline
3. Maintain the existing classes for consistent styling

### Tailwind CSS Classes Explained

#### Responsive Design Classes
- `md:` prefix indicates styles that apply on medium screens and larger
- Example: `text-4xl md:text-6xl` means:
  - `text-4xl` (smaller text) on mobile
  - `text-6xl` (larger text) on medium screens and up

#### Common Class Patterns
```html
<!-- Example of spacing classes -->
<div class="mb-8 px-6 py-4">
```
- `mb-8`: Margin bottom (spacing)
- `px-6`: Padding left and right
- `py-4`: Padding top and bottom

## Fixing Broken Links

### Navigation Menu Links
Current placeholder links in the header:
```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Portfolio</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Services</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">About</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Contact</a>
</div>
```

To update links:
1. Replace `#` with your actual page URLs
2. Example:
```html
<a href="portfolio.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Portfolio</a>
```

### Footer Links
Locate the footer section and update social media links:
```html
<div class="flex space-x-4">
    <a href="https://instagram.com/yourhandle" class="text-gray-400 hover:text-white transition duration-300">
        <i class="fab fa-instagram"></i>
    </a>
</div>
```

## Adding Privacy and Terms Pages

### Step 1: Create New Footer Section
Add this code before the copyright notice:
```html
<div class="mt-8 text-center">
    <a href="privacy.html" class="text-gray-400 hover:text-white transition duration-300 mr-4">Privacy Policy</a>
    <a href="terms.html" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a>
</div>
```

### Step 2: Style Consistency
Ensure new links match existing footer styles:
- Use `text-gray-400` for normal state
- Use `hover:text-white` for hover state
- Add `transition duration-300` for smooth effects

## Troubleshooting

### Common Issues

1. **Broken Responsive Layout**
   - Check for missing `md:` prefixes in classes
   - Verify container classes are present: `container mx-auto px-6`

2. **Missing Icons**
   - Ensure Font Awesome CSS is properly linked
   - Verify icon class names (e.g., `fas fa-star`)

3. **Link Issues**
   - Confirm file paths are correct
   - Use relative paths for internal links
   - Use full URLs for external links

### Need Help?
- Check the [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Verify HTML syntax at [W3C Validator](https://validator.w3.org/)
- Test responsive design using browser developer tools

Remember to:
- Back up your files before making changes
- Test all links after updates
- View changes on multiple devices
- Keep consistent styling throughout

This guide specifically references your landing page structure. For additional customization needs, please refer to the Tailwind CSS documentation or consult a web developer.