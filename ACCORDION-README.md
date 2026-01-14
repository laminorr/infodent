# Professional Accordion Section for Elementor

A beautiful, responsive accordion component designed to match your "How We Work" section design, ready to integrate with Elementor.

## 📁 Files Included

- **accordion.html** - Standalone HTML file (preview/testing)
- **accordion-elementor.html** - Code optimized for Elementor HTML widget
- **ACCORDION-README.md** - This file with complete instructions

## 🚀 How to Use in Elementor

### Method 1: Using HTML Widget (Recommended)

1. **Open Elementor Editor**
   - Edit the page where you want to add the accordion
   - Click "Edit with Elementor"

2. **Add HTML Widget**
   - Drag and drop the "HTML" widget from the left sidebar to your desired location
   - The HTML widget is usually found under "General" or "WordPress" widgets

3. **Insert the Code**
   - Open the file `accordion-elementor.html`
   - Copy ALL the content (Ctrl+A, then Ctrl+C)
   - Paste it into the HTML widget's code editor

4. **Adjust Settings**
   - In the widget settings, you can adjust:
     - Width (set to "Full Width" for best results)
     - Margins and padding as needed

5. **Update/Publish**
   - Click "Update" or "Publish" at the bottom left
   - View your page to see the accordion in action!

### Method 2: Using Custom Code (Alternative)

If you prefer to add the code to your theme:

1. Go to **Appearance → Theme File Editor**
2. Add the CSS from `accordion-elementor.html` to your theme's style.css
3. Add the HTML structure where needed in your template
4. Add the JavaScript to your theme's functions or footer

## 🎨 Customization Guide

### Change Colors

Find these lines in the CSS section and modify the hex colors:

```css
/* First section - lightest beige */
background: linear-gradient(90deg, #f5ebe0 0%, #f5ebe0 75%, transparent 75%);

/* Second section - slightly darker */
background: linear-gradient(90deg, #e8ddd0 0%, #e8ddd0 75%, transparent 75%);

/* Third section - medium beige */
background: linear-gradient(90deg, #dcd1c1 0%, #dcd1c1 75%, transparent 75%);

/* Fourth section - darkest beige */
background: linear-gradient(90deg, #d0c5b2 0%, #d0c5b2 75%, transparent 75%);
```

### Change Font Styles

Modify these CSS properties:

```css
.custom-accordion .accordion-header h2 {
    font-size: 48px;        /* Title size */
    font-style: italic;     /* Change to 'normal' for non-italic */
    font-weight: 400;       /* Font weight (100-900) */
    font-family: 'Your Font', serif;  /* Change font family */
}

.custom-accordion .accordion-content p {
    font-size: 18px;        /* Content text size */
    line-height: 1.8;       /* Line spacing */
}
```

### Change Titles and Content

In the HTML section, find and modify:

```html
<h2>How We Work...</h2>  <!-- Change title here -->
<p>Your custom content here...</p>  <!-- Change content here -->
```

### Add More Accordion Items

Copy and paste this block before the closing `</div>` of `custom-accordion`:

```html
<!-- Accordion Item 5 -->
<div class="accordion-item">
    <div class="accordion-header">
        <h2>Your New Title</h2>
    </div>
    <div class="accordion-content">
        <p>Your new content goes here.</p>
    </div>
</div>
```

Then add corresponding CSS for the new item:

```css
.custom-accordion .accordion-item:nth-child(5) .accordion-header {
    background: linear-gradient(90deg, #c4b9a6 0%, #c4b9a6 75%, transparent 75%);
}
```

## 📱 Responsive Design

The accordion is fully responsive and automatically adjusts for:

- **Desktop** (> 768px): Full size with 48px titles
- **Tablet** (≤ 768px): Medium size with 32px titles
- **Mobile** (≤ 480px): Compact size with 24px titles

## ✨ Features

- ✅ Smooth expand/collapse animation
- ✅ One section open at a time
- ✅ First section opens by default
- ✅ Curved edge design on the right
- ✅ Gradient background colors
- ✅ Fully responsive
- ✅ Hover effects
- ✅ Works with Elementor preview mode
- ✅ No jQuery dependency (vanilla JavaScript)

## 🔧 Troubleshooting

### Accordion not working?

1. **Check if code is complete**: Make sure you copied ALL the code including `<style>`, HTML, and `<script>` sections
2. **Clear cache**: Clear your browser cache and WordPress cache
3. **Check Elementor settings**: Ensure the HTML widget allows custom code
4. **Console errors**: Open browser developer tools (F12) and check for JavaScript errors

### Styling issues?

1. **CSS conflicts**: Your theme might have conflicting styles. Try adding `!important` to specific CSS rules
2. **Width issues**: Set the Elementor section/column to "Full Width"
3. **Font not showing**: Make sure the font family is available on your site

### Animation not smooth?

1. Check if there are any jQuery animations conflicting
2. Try adjusting the transition timing in CSS:
   ```css
   transition: max-height 0.4s ease-out, padding 0.4s ease-out;
   ```

## 📞 Support

Need help? Common issues:

1. **White space issues**: Adjust padding in Elementor section settings
2. **Not mobile responsive**: Clear cache and test in incognito mode
3. **Click not working**: Check if there are overlapping elements

## 🎯 Browser Compatibility

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 License

Free to use for personal and commercial projects.

## 🔄 Version

Version 1.0 - January 2026

---

**Pro Tip**: Always test in Elementor preview mode and on actual devices before publishing!
