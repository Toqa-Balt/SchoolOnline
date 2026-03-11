# Lab 8: Frontend HTML & CSS - Homework Assignment

## Overview

This homework assignment reinforces HTML5 and CSS3 fundamentals. You'll practice creating semantic HTML structures, styling with CSS, implementing responsive design, using Flexbox and Grid, and ensuring accessibility.

## Learning Objectives

By completing this homework, you will:
- Create semantic HTML5 document structures
- Style web pages with CSS selectors and properties
- Implement responsive layouts with media queries
- Use CSS Flexbox for flexible layouts
- Use CSS Grid for complex layouts
- Design and style forms with proper validation
- Ensure web accessibility (WCAG guidelines)
- Add CSS animations and transitions
- Apply modern web design best practices

## Prerequisites

- Completed Lab 8: Frontend HTML & CSS
- Understanding of HTML5 semantic elements
- Familiarity with CSS selectors and properties
- Knowledge of responsive design principles
- Basic understanding of web accessibility

---

## Assignment 1: Online School Landing Page

### Task
Create a complete landing page for the Online School using semantic HTML and modern CSS.

### Requirements

#### HTML Structure

1. **Create `index.html`** with proper document structure:
   - DOCTYPE declaration
   - `<html lang="en">`
   - `<head>` with meta tags:
     - charset UTF-8
     - viewport for responsive design
     - title and description
     - link to stylesheet
   - Semantic structure:
     - `<header>` with navigation
     - `<main>` with multiple sections
     - `<footer>` with copyright and links

2. **Navigation Bar** (`<nav>`):
   - Logo/brand name
   - Navigation links: Home, Courses, Students, Teachers, About, Contact
   - Responsive hamburger menu for mobile (CSS only)

3. **Hero Section** (`<section class="hero">`):
   - Heading: "Welcome to Online School"
   - Subheading: "Learn from anywhere, anytime"
   - Call-to-action button: "Get Started"
   - Background image or gradient

4. **Features Section** (`<section class="features">`):
   - Heading: "Why Choose Us"
   - Three feature cards with:
     - Icon (use Font Awesome or Unicode)
     - Title
     - Description
   - Use CSS Grid for layout

5. **Courses Section** (`<section class="courses">`):
   - Heading: "Popular Courses"
   - Course cards (minimum 6) with:
     - Course image
     - Course title
     - Instructor name
     - Duration
     - Enrollment button
   - Use CSS Grid with responsive columns

6. **Statistics Section** (`<section class="stats">`):
   - Four stat boxes showing:
     - Number of students
     - Number of courses
     - Number of teachers
     - Success rate
   - Use Flexbox for layout
   - Add counter animation (CSS)

7. **Testimonials Section** (`<section class="testimonials">`):
   - Heading: "What Our Students Say"
   - Three testimonial cards with:
     - Student photo
     - Quote
     - Student name and course
   - Use Flexbox or Grid

8. **Footer** (`<footer>`):
   - Three columns:
     - About section with description
     - Quick links
     - Contact information
   - Social media icons
   - Copyright notice

#### CSS Styling

9. **Create `css/styles.css`** with:
   - CSS Reset or Normalize
   - CSS Custom Properties (variables) for:
     - Colors (primary, secondary, text, background)
     - Fonts (headings, body)
     - Spacing (margins, padding)
     - Breakpoints
   - Typography styles
   - Layout styles
   - Component styles

10. **Color Scheme**:
    - Define a professional color palette
    - Primary color for branding
    - Secondary color for accents
    - Neutral colors for text and backgrounds
    - Use CSS variables

11. **Typography**:
    - Import Google Fonts (2-3 fonts max)
    - Define font sizes using rem units
    - Set line heights for readability
    - Style headings (h1-h6)
    - Style paragraphs and lists

12. **Navigation Styling**:
    - Fixed or sticky navigation
    - Hover effects on links
    - Active state styling
    - Smooth transitions
    - Mobile hamburger menu (CSS only)

13. **Hero Section Styling**:
    - Full viewport height
    - Centered content
    - Background image with overlay
    - Or gradient background
    - Animated entrance (CSS animation)

14. **Card Components**:
    - Consistent card design
    - Box shadows
    - Border radius
    - Hover effects (lift, scale, shadow)
    - Smooth transitions

15. **Buttons**:
    - Primary and secondary button styles
    - Hover and active states
    - Disabled state
    - Smooth transitions
    - Consistent sizing

#### Responsive Design

16. **Create `css/responsive.css`** with media queries:
    - Mobile first approach
    - Breakpoints:
      - Mobile: < 768px
      - Tablet: 768px - 1024px
      - Desktop: > 1024px
    - Responsive navigation
    - Responsive grid layouts
    - Responsive typography
    - Hide/show elements based on screen size

17. **Mobile Optimization**:
    - Stack sections vertically
    - Single column layouts
    - Larger touch targets (min 44x44px)
    - Readable font sizes (min 16px)
    - Optimized images

#### Animations

18. **Create `css/animations.css`** with:
    - Fade in animations for sections
    - Slide in animations for cards
    - Hover animations for buttons and cards
    - Loading animations
    - Smooth scroll behavior

### Expected Deliverables
- index.html (semantic HTML structure)
- css/styles.css (main stylesheet)
- css/responsive.css (media queries)
- css/animations.css (animations and transitions)
- images/ folder with optimized images
- README.md explaining design choices

---

## Assignment 2: Student Registration Form

### Task
Create a comprehensive student registration form with proper validation and styling.

### Requirements

#### HTML Structure

1. **Create `register.html`** with:
   - Semantic form structure
   - Proper form elements
   - Labels for all inputs
   - Fieldsets for grouping
   - Validation attributes

2. **Form Sections**:
   - Personal Information:
     - First Name (required, text)
     - Last Name (required, text)
     - Date of Birth (required, date)
     - Gender (required, radio buttons)
   - Contact Information:
     - Email (required, email validation)
     - Phone (required, tel validation)
     - Address (textarea)
     - City (required, text)
     - State/Province (required, select)
     - Zip Code (required, pattern validation)
   - Academic Information:
     - Previous Education (required, select)
     - Intended Major (required, select)
     - Start Date (required, date)
     - Full-time/Part-time (required, radio)
   - Additional Information:
     - How did you hear about us? (select)
     - Comments (textarea, optional)
     - Terms and Conditions (required, checkbox)
     - Newsletter subscription (checkbox, optional)

3. **Form Controls**:
   - Submit button
   - Reset button
   - Required field indicator (*)
   - Form validation messages

#### CSS Styling

4. **Form Layout**:
   - Two-column layout on desktop
   - Single column on mobile
   - Consistent spacing
   - Clear visual hierarchy

5. **Input Styling**:
   - Consistent input heights
   - Border and focus states
   - Placeholder styling
   - Disabled state styling
   - Error state styling
   - Success state styling

6. **Label Styling**:
   - Clear association with inputs
   - Required field indicators
   - Proper spacing
   - Readable font size

7. **Button Styling**:
   - Primary button for submit
   - Secondary button for reset
   - Hover and active states
   - Disabled state
   - Loading state (optional)

8. **Validation Styling**:
   - Error messages in red
   - Success indicators in green
   - Invalid input borders
   - Valid input borders
   - Focus states

#### Accessibility

9. **Form Accessibility**:
   - Proper label associations (for/id)
   - ARIA labels where needed
   - Keyboard navigation support
   - Focus indicators
   - Error announcements
   - Logical tab order

10. **Semantic HTML**:
    - Use `<fieldset>` and `<legend>`
    - Use appropriate input types
    - Use `<label>` for all inputs
    - Use `required` attribute
    - Use `pattern` for validation

### Expected Deliverables
- register.html (registration form)
- css/form-styles.css (form-specific styles)
- Fully functional form with validation
- Responsive design
- Accessible form

---

## Assignment 3: Course Catalog Page

### Task
Create a course catalog page with filtering, sorting, and responsive card layout.

### Requirements

#### HTML Structure

1. **Create `courses.html`** with:
   - Page header with title
   - Filter sidebar
   - Course grid/list
   - Pagination

2. **Filter Sidebar**:
   - Search input
   - Category checkboxes:
     - Computer Science
     - Mathematics
     - Business
     - Arts
     - Sciences
   - Level radio buttons:
     - Beginner
     - Intermediate
     - Advanced
   - Duration range slider (optional)
   - Apply Filters button
   - Clear Filters button

3. **Course Cards** (minimum 12 courses):
   - Course image
   - Course title
   - Instructor name with photo
   - Category badge
   - Level badge
   - Duration
   - Rating (stars)
   - Price
   - Short description
   - Enroll button

4. **Sorting Options**:
   - Sort by: Popularity, Rating, Price, Duration
   - View toggle: Grid view / List view

5. **Pagination**:
   - Page numbers
   - Previous/Next buttons
   - Items per page selector

#### CSS Styling

6. **Layout**:
   - Sidebar + main content layout
   - Use CSS Grid or Flexbox
   - Responsive: sidebar collapses on mobile
   - Sticky sidebar on desktop

7. **Course Cards**:
   - Grid layout: 3 columns on desktop, 2 on tablet, 1 on mobile
   - Consistent card height
   - Image aspect ratio maintained
   - Hover effects
   - Smooth transitions

8. **Filter Sidebar**:
   - Styled checkboxes and radio buttons
   - Styled search input
   - Collapsible sections (CSS only)
   - Clear visual feedback

9. **Badges**:
   - Category badges with different colors
   - Level badges (Beginner: green, Intermediate: yellow, Advanced: red)
   - Rounded corners
   - Consistent sizing

10. **Rating Stars**:
    - Star icons (Font Awesome or Unicode)
    - Filled and empty states
    - Half-star support (optional)
    - Color: gold/yellow

#### Responsive Design

11. **Mobile Layout**:
    - Filter sidebar becomes top bar with dropdown
    - Single column card layout
    - Larger touch targets
    - Simplified card design

12. **Tablet Layout**:
    - Two column card layout
    - Sidebar remains visible
    - Adjusted spacing

### Expected Deliverables
- courses.html (course catalog page)
- css/courses.css (page-specific styles)
- Responsive grid layout
- Functional filters (CSS only, no JavaScript)
- Accessible design

---

## Bonus Challenges (Optional)

### Challenge 1: CSS-Only Accordion
Create an FAQ page with CSS-only accordion:
- Use checkbox hack or :target pseudo-class
- Smooth expand/collapse animations
- Accessible keyboard navigation
- Multiple sections

### Challenge 2: CSS-Only Modal
Create a modal dialog using only CSS:
- Use :target pseudo-class
- Overlay background
- Close button
- Smooth fade-in animation
- Accessible focus management

### Challenge 3: CSS-Only Image Gallery
Create an image gallery with:
- Grid layout
- Lightbox effect (CSS only)
- Image captions
- Hover effects
- Responsive design

### Challenge 4: CSS-Only Tabs
Create tabbed content interface:
- Use radio buttons and labels
- Smooth transitions
- Active tab styling
- Responsive design
- Accessible

### Challenge 5: Dark Mode Toggle
Implement dark mode:
- Use CSS custom properties
- Toggle with checkbox (CSS only)
- Smooth color transitions
- Save preference (requires JavaScript, optional)
- Accessible contrast ratios

---

## Running Your Pages

### Local Development

1. **Open HTML files in browser**:
```bash
open index.html
# or
open register.html
# or
open courses.html
```

2. **Use Live Server** (VS Code extension):
   - Install Live Server extension
   - Right-click HTML file
   - Select "Open with Live Server"

3. **Use Python HTTP Server**:
```bash
python -m http.server 8000
# Then open http://localhost:8000
```

### Testing

1. **Test in multiple browsers**:
   - Chrome
   - Firefox
   - Safari
   - Edge

2. **Test responsive design**:
   - Use browser DevTools
   - Test on actual devices
   - Test different screen sizes

3. **Test accessibility**:
   - Use browser accessibility tools
   - Test keyboard navigation
   - Test with screen reader
   - Check color contrast

---

## Submission Checklist

Before submitting, ensure you have:

- [ ] All HTML files with semantic structure
- [ ] All CSS files organized and commented
- [ ] Responsive design working on all screen sizes
- [ ] All images optimized and included
- [ ] Forms with proper validation
- [ ] Accessible design (WCAG AA compliance)
- [ ] Cross-browser compatibility
- [ ] No console errors
- [ ] Clean, well-formatted code
- [ ] README.md with project description
- [ ] Screenshots of final pages

### File Structure
```
homework/
├── index.html
├── register.html
├── courses.html
├── css/
│   ├── styles.css
│   ├── responsive.css
│   ├── animations.css
│   ├── form-styles.css
│   └── courses.css
├── images/
│   ├── hero-bg.jpg
│   ├── course-*.jpg
│   └── icons/
├── fonts/ (if using local fonts)
└── README.md
```

---

## Code Quality Guidelines

### HTML Best Practices

1. **Semantic HTML**:
   ```html
   <!-- Good -->
   <header>
       <nav>
           <ul>
               <li><a href="/">Home</a></li>
           </ul>
       </nav>
   </header>
   
   <!-- Bad -->
   <div class="header">
       <div class="nav">
           <div class="menu">
               <div><a href="/">Home</a></div>
           </div>
       </div>
   </div>
   ```

2. **Accessibility**:
   ```html
   <!-- Good -->
   <label for="email">Email:</label>
   <input type="email" id="email" name="email" required>
   
   <!-- Bad -->
   <div>Email:</div>
   <input type="text" name="email">
   ```

### CSS Best Practices

1. **CSS Variables**:
   ```css
   :root {
       --primary-color: #007bff;
       --secondary-color: #6c757d;
       --text-color: #333;
       --bg-color: #fff;
       --spacing-unit: 1rem;
   }
   
   .button {
       background-color: var(--primary-color);
       padding: var(--spacing-unit);
   }
   ```

2. **Mobile-First Media Queries**:
   ```css
   /* Mobile styles (default) */
   .container {
       width: 100%;
       padding: 1rem;
   }
   
   /* Tablet */
   @media (min-width: 768px) {
       .container {
           width: 750px;
           margin: 0 auto;
       }
   }
   
   /* Desktop */
   @media (min-width: 1024px) {
       .container {
           width: 960px;
       }
   }
   ```

3. **Flexbox Layout**:
   ```css
   .navbar {
       display: flex;
       justify-content: space-between;
       align-items: center;
       padding: 1rem;
   }
   
   .nav-links {
       display: flex;
       gap: 2rem;
       list-style: none;
   }
   ```

4. **Grid Layout**:
   ```css
   .course-grid {
       display: grid;
       grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
       gap: 2rem;
       padding: 2rem;
   }
   ```

---

## Common Pitfalls to Avoid

- ❌ Using `<div>` for everything instead of semantic elements
- ❌ Not using labels for form inputs
- ❌ Forgetting viewport meta tag
- ❌ Using fixed pixel widths instead of responsive units
- ❌ Not testing on mobile devices
- ❌ Poor color contrast (accessibility issue)
- ❌ Not optimizing images
- ❌ Inline styles instead of external CSS
- ❌ Not using CSS variables for consistency
- ❌ Forgetting alt text for images
- ❌ Not testing keyboard navigation
- ❌ Using tables for layout

---

## Tips for Success

1. **Start with HTML structure** - Get the content right first
2. **Use semantic elements** - They improve accessibility and SEO
3. **Mobile-first approach** - Design for mobile, then enhance for desktop
4. **Test frequently** - Check your work in browser often
5. **Use browser DevTools** - Inspect elements and debug CSS
6. **Validate your code** - Use W3C validators
7. **Optimize images** - Compress before using
8. **Comment your code** - Explain complex CSS
9. **Keep it simple** - Don't over-complicate
10. **Learn from examples** - Study well-designed websites

---

## Resources

### Documentation
- [MDN Web Docs](https://developer.mozilla.org/)
- [HTML5 Specification](https://html.spec.whatwg.org/)
- [CSS Specification](https://www.w3.org/Style/CSS/)
- [Web Accessibility Guidelines](https://www.w3.org/WAI/WCAG21/quickref/)

### Tools
- [CSS-Tricks](https://css-tricks.com/)
- [Can I Use](https://caniuse.com/) - Browser compatibility
- [Google Fonts](https://fonts.google.com/)
- [Font Awesome](https://fontawesome.com/) - Icons
- [Coolors](https://coolors.co/) - Color palette generator
- [TinyPNG](https://tinypng.com/) - Image compression

### Validators
- [W3C HTML Validator](https://validator.w3.org/)
- [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
- [WAVE Accessibility Tool](https://wave.webaim.org/)

### Learning Resources
- Lab 8 LAB_8_FRONTEND_HTML_CSS.md
- [Flexbox Froggy](https://flexboxfroggy.com/) - Learn Flexbox
- [Grid Garden](https://cssgridgarden.com/) - Learn CSS Grid

---

## Questions and Support

If you encounter issues:

1. **Check HTML/CSS syntax** - Use validators
2. **Use browser DevTools** - Inspect and debug
3. **Test in different browsers** - Ensure compatibility
4. **Check responsive design** - Test different screen sizes
5. **Verify accessibility** - Use accessibility tools
6. **Review documentation** - MDN is your friend
7. **Ask for help** - Reach out during office hours

---

**Remember: Good HTML and CSS are the foundation of web development. Master these fundamentals before moving to JavaScript frameworks!** 🎨🚀
