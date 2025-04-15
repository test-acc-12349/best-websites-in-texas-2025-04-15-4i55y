# Landing Page Maintenance Guide
## Best Websites TX Landing Page Documentation

This guide provides detailed instructions for maintaining and customizing the Best Websites TX landing page. Whether you're new to web development or need a quick reference, follow these step-by-step instructions.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Header Section
The header contains the company name and navigation menu:

```html
<div class="text-2xl font-bold text-blue-600">
    Best Websites TX  <!-- Update company name here -->
</div>
```

To modify:
1. Locate this section at the top of the page
2. Change "Best Websites TX" to your desired text
3. Adjust text size by modifying `text-2xl` (options: text-sm, text-base, text-lg, text-2xl, text-3xl)
4. Change color by updating `text-blue-600` (options: text-[color]-[shade], e.g., text-red-500)

### Hero Section
The main headline and subheading are located in:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight mb-6">
    Best Websites In Texas  <!-- Main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    Custom Websites For Your Business  <!-- Subheading -->
</p>
```

Understanding the classes:
- `text-4xl md:text-5xl lg:text-6xl`: Responsive text sizing (mobile, tablet, desktop)
- `mb-6`: Margin bottom spacing (6 units)
- `text-gray-900`: Dark gray text color

### Features Section
Each feature card follows this structure:

```html
<div class="bg-white rounded-xl p-8 shadow-lg hover:shadow-xl transition-shadow duration-300">
    <div class="text-blue-600 mb-4">
        <i class="fas fa-magic text-3xl"></i>  <!-- Icon -->
    </div>
    <h3 class="text-xl font-bold mb-4">Easy to Use</h3>  <!-- Feature title -->
    <p class="text-gray-600">Intuitive interface...</p>  <!-- Feature description -->
</div>
```

To modify features:
1. Locate the features section (id="features")
2. Update icon by changing `fa-magic` to any [Font Awesome](https://fontawesome.com/icons) icon
3. Modify title and description text as needed
4. Maintain the existing classes for consistent styling

## Fixing Broken Links

### Navigation Menu Links
Current navigation links are:

```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

To update:
1. Ensure internal links match section IDs (e.g., `href="#features"` points to `id="features"`)
2. For external links, replace "#" with full URL: `href="https://example.com"`
3. Test all links after updating

### Call-to-Action Links
The main CTA buttons currently point to:

```html
<a href="https://sigmaseo.io" class="inline-block bg-blue-600...">
    Get Started Today
</a>
```

To modify:
1. Replace "https://sigmaseo.io" with your desired URL
2. Update button text as needed
3. Maintain the existing classes for styling

## Linking Privacy and Terms Pages

### Footer Legal Links
Current placeholder links:

```html
<div>
    <h4 class="text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To add privacy and terms pages:
1. Create privacy.html and terms.html in your root directory
2. Update the links:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

Common issues and solutions:

1. **Broken Internal Links**
   - Ensure section IDs match exactly (case-sensitive)
   - Check for extra spaces in href attributes
   - Verify all sections have unique IDs

2. **Responsive Design Issues**
   - Don't remove `md:` or `lg:` prefixes from classes
   - Maintain the existing responsive class structure
   - Test on multiple screen sizes

3. **Icon Not Displaying**
   - Verify Font Awesome CDN link in header
   - Check icon class names against Font Awesome documentation
   - Ensure proper icon prefix (fas, far, fab)

For additional help or questions, please contact your web development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).