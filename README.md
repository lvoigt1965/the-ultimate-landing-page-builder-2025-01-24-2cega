# Landing Page Maintenance Guide

This guide will help you customize and maintain your landing page. Follow these instructions carefully to make updates while preserving the design and functionality.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your logo and navigation menu. To update:

1. Change the logo text:
```html
<!-- Find this line in the header -->
<a href="/" class="text-2xl font-bold bg-gradient-to-r from-purple-600 to-blue-500 bg-clip-text text-transparent">
    PageBuilder  <!-- Change this text -->
</a>
```

2. Modify navigation menu items:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>  <!-- Change text here -->
    <a href="#benefits">Benefits</a>  <!-- And here -->
    <a href="#faq">FAQ</a>           <!-- And here -->
</div>
```

### Hero Section
Update the main headline and subheading:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-8 bg-gradient-to-r from-purple-600 to-blue-500 bg-clip-text text-transparent">
    The Ultimate Landing Page Builder  <!-- Change main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    Create stunning landing pages in minutes  <!-- Change subheading -->
</p>
```

### Understanding Tailwind Classes
Common classes explained:
- `text-4xl`: Large text size
- `md:text-5xl`: Larger text on medium screens
- `font-bold`: Bold text weight
- `mb-8`: Bottom margin spacing
- `bg-white`: White background
- `text-gray-600`: Gray text color

To modify spacing:
- Increase margins: Change `mb-8` to `mb-12` for more space
- Adjust padding: Change `p-8` to `p-4` for less padding

## Managing Links

### Navigation Links
Update the navigation menu links:
```html
<!-- In the header section -->
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>  <!-- Links to features section -->
    <a href="#benefits">Benefits</a>  <!-- Links to benefits section -->
    <a href="#faq">FAQ</a>           <!-- Links to FAQ section -->
</div>
```

### Call-to-Action Buttons
Replace the default links:
```html
<!-- Find all instances of -->
<a href="https://orlandi.com.au">
<!-- Replace with your desired URL -->
<a href="https://your-website.com">
```

### Social Media Links
Update social media links in the footer:
```html
<div class="flex space-x-4">
    <a href="#" class="hover:text-white transition-colors duration-300">
        <!-- Replace # with your social media URL -->
        <a href="https://twitter.com/your-handle">
</div>
```

## Adding Privacy and Terms Pages

### 1. Create New Pages
Create two new files in your project:
- `privacy.html`
- `terms.html`

### 2. Update Footer Links
Replace the placeholder links:
```html
<!-- In the footer section -->
<ul class="space-y-2 text-sm">
    <li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
    <li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
</ul>
```

### 3. Maintain Consistent Styling
Copy these classes for new links:
```html
class="hover:text-white transition-colors duration-300"
```

## Troubleshooting

### Common Issues

1. **Broken Navigation Links**
   - Ensure section IDs match href attributes
   - Example: `href="#features"` needs matching `id="features"` in section

2. **Responsive Design Issues**
   - Check mobile display using browser dev tools
   - Verify `md:` and `lg:` prefixed classes are correct

3. **Gradient Text Not Showing**
   - Ensure all these classes are present:
```html
bg-gradient-to-r from-purple-600 to-blue-500 bg-clip-text text-transparent
```

### Need Help?
- Inspect elements using browser developer tools (Right-click → Inspect)
- Check the Tailwind CSS documentation for class references
- Verify all files are in the correct directory
- Test all links after making changes

Remember to:
- Back up your files before making changes
- Test on multiple devices and browsers
- Keep original class names for reference
- Maintain consistent spacing and indentation

For additional support, contact: lyndon.voigt@gmail.com