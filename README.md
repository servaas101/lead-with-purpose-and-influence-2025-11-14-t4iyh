# Leadership Academy Landing Page - Maintenance & Customization Guide

Welcome! This comprehensive guide will help you maintain, update, and customize your Leadership Academy landing page. Whether you're making simple text changes or adding new sections, this document provides step-by-step instructions tailored to your specific HTML structure.

---

## Table of Contents

1. [Quick Start Guide](#quick-start-guide)
2. [Understanding Your Page Structure](#understanding-your-page-structure)
3. [Updating Text Content](#updating-text-content)
4. [Modifying Styles with Tailwind CSS](#modifying-styles-with-tailwind-css)
5. [Fixing and Managing Links](#fixing-and-managing-links)
6. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
7. [Common Customizations](#common-customizations)
8. [Troubleshooting](#troubleshooting)
9. [Best Practices](#best-practices)

---

## Quick Start Guide

### What You Need to Know

This landing page uses:
- **HTML**: The structure and content of your page
- **Tailwind CSS**: A utility-based styling framework that uses pre-made classes
- **Font Awesome**: Icons used throughout the page
- **Google Fonts**: Custom fonts (Space Grotesk and Inter)
- **Web3Forms**: For the contact form functionality

### Files You'll Be Working With

- `index.html` - Your main landing page (the file provided)
- `privacy.html` - Privacy policy page (you'll create this)
- `terms.html` - Terms of service page (you'll create this)

### Making Your First Change

1. Open `index.html` in a text editor (VS Code, Notepad++, or even Notepad)
2. Use `Ctrl+F` (or `Cmd+F` on Mac) to search for text you want to change
3. Replace the old text with new text
4. Save the file (`Ctrl+S`)
5. Refresh your browser to see the changes

---

## Understanding Your Page Structure

### The Anatomy of Your Landing Page

Your page is organized into distinct sections. Here's what each section does:

```
Header (Navigation Bar)
    ↓
Hero Section (Large welcome area with main message)
    ↓
Features Section (3 feature cards)
    ↓
Benefits Section (4 benefit cards)
    ↓
Testimonials Section (4 customer testimonials)
    ↓
About Us Section (Company information)
    ↓
FAQ Section (Frequently Asked Questions)
    ↓
CTA Section (Call-to-Action - "Ready to Transform?")
    ↓
Contact Section (Contact form)
    ↓
Footer (Links and company info)
```

### Color Scheme

Your page uses a specific color palette:

- **Primary Red**: `#FF5A5F` - Used for main buttons and accents
- **Primary Yellow**: `#FFD166` - Used for secondary accents
- **Dark Text**: `#1A1A1A` - Main text color
- **Light Gray**: `#F3F4F6` - Background for alternating sections
- **Medium Gray**: `#666666` - Secondary text

### Typography

- **Headings**: Space Grotesk font (bold, modern look)
- **Body Text**: Inter font (clean, readable)

---

## Updating Text Content

### Finding and Replacing Text

The easiest way to update content is using Find & Replace:

1. Open your `index.html` file
2. Press `Ctrl+H` (or `Cmd+H` on Mac) to open Find & Replace
3. Enter the text you want to find
4. Enter the replacement text
5. Click "Replace All" or review each instance first

### Section-by-Section Text Updates

#### 1. **Header/Navigation Text**

**Location**: Lines 72-86 (approximately)

```html
<!-- Current Navigation Links -->
<a href="#features" class="text-[#1A1A1A] font-light hover:text-[#FF5A5F] transition-colors duration-300">Features</a>
<a href="#benefits" class="text-[#1A1A1A] font-light hover:text-[#FF5A5F] transition-colors duration-300">Benefits</a>
<a href="#testimonials" class="text-[#1A1A1A] font-light hover:text-[#FF5A5F] transition-colors duration-300">Testimonials</a>
<a href="#faq" class="text-[#1A1A1A] font-light hover:text-[#FF5A5F] transition-colors duration-300">FAQ</a>
```

**To change navigation text:**
- Find: `Features` → Replace with your new text (e.g., "Courses")
- Find: `Benefits` → Replace with your new text (e.g., "Why Us")
- The same applies to Testimonials and FAQ

**Pro Tip**: The navigation appears twice—once in the desktop menu and once in the mobile menu. When you use Find & Replace, it will update both automatically.

---

#### 2. **Hero Section (Main Welcome Message)**

**Location**: Lines 100-120 (approximately)

**Current content:**
```html
<h1 class="text-5xl md:text-6xl lg:text-7xl heading-primary text-[#1A1A1A] leading-tight mb-6">
    Lead With <span class="text-[#FF5A5F]">Purpose</span> and <span class="text-[#FFD166]">Influence</span>
</h1>

<p class="text-xl md:text-2xl text-light text-[#1A1A1A] mb-8 leading-relaxed">
    Transform Your Skills. Lead With Confidence.
</p>

<p class="text-lg text-light text-gray-600 mb-10 leading-relaxed">
    Discover a transformative learning experience designed to elevate your leadership capabilities...
</p>
```

**To update the main headline:**
1. Find the `<h1>` tag (the largest heading)
2. Replace "Lead With Purpose and Influence" with your headline
3. **Important**: Keep the `<span>` tags for colored words:
   - Text in `<span class="text-[#FF5A5F]">` appears in red
   - Text in `<span class="text-[#FFD166]">` appears in yellow

**Example - If you want to change to "Build Your Leadership Legacy":**
```html
<h1 class="text-5xl md:text-6xl lg:text-7xl heading-primary text-[#1A1A1A] leading-tight mb-6">
    Build Your <span class="text-[#FF5A5F]">Leadership</span> <span class="text-[#FFD166]">Legacy</span>
</h1>
```

---

#### 3. **Features Section**

**Location**: Lines 140-200 (approximately)

Each feature card has three parts: icon, title, and description.

**Current structure for Feature 1:**
```html
<div class="card-hover bg-white p-8 shadow-md">
    <div class="w-12 h-12 bg-gradient-to-br from-[#FF5A5F] to-[#FFD166] rounded-lg flex items-center justify-center mb-6">
        <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24" stroke-width="1.5">
            <path stroke-linecap="round" stroke-linejoin="round" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path>
        </svg>
    </div>
    <h3 class="text-2xl heading-primary text-[#1A1A1A] mb-3">Self-Awareness Mastery</h3>
    <p class="text-light text-gray-600">
        Develop profound self-awareness through evidence-based assessments...
    </p>
</div>
```

**To update Feature 1 title and description:**
1. Find: `Self-Awareness Mastery`
2. Replace with your new title (e.g., "Expert Coaching")
3. Find the paragraph below it and replace the description text

**Note**: Don't modify the `<svg>` code (the icon). If you want to change icons, see the "Changing Icons" section below.

---

#### 4. **Benefits Section**

**Location**: Lines 220-280 (approximately)

Each benefit has:
- An icon (don't modify the SVG)
- A title (easy to change)
- A description (easy to change)

**To update Benefit 1 ("Learn on Your Schedule"):**
1. Find: `Learn on Your Schedule`
2. Replace with your new title
3. Find the paragraph starting with "Access premium content..." and replace it

---

#### 5. **Testimonials Section**

**Location**: Lines 340-420 (approximately)

Each testimonial card contains:
- Star ratings (don't change these)
- Quote text (the testimonial itself)
- Person's name
- Person's title/company

**To update the first testimonial:**
1. Find: `"The Leadership Academy transformed how I approach challenges..."`
2. Replace with new testimonial text
3. Find: `Sarah Mitchell` → Replace with new person's name
4. Find: `Senior Manager, Tech Solutions Inc.` → Replace with new title/company

**Important**: Keep the quotation marks around the testimonial text.

---

#### 6. **About Us Section**

**Location**: Lines 430-460 (approximately)

**Current content:**
```html
<h2 class="text-4xl md:text-5xl heading-primary text-[#1A1A1A] mb-4">
    About Leadership Academy
</h2>

<p class="text-lg text-light text-gray-600 leading-relaxed">
    Founded in 2018 by a collective of executive coaches...
</p>

<p class="text-lg text-light text-gray-600 leading-relaxed">
    Our mission is to cultivate purposeful, influential leaders...
</p>
```

**To update your About Us:**
1. Find: `About Leadership Academy` → Replace with your heading
2. Find: `Founded in 2018...` → Replace with your company's founding story
3. Find: `Our mission is to cultivate...` → Replace with your mission statement

---

#### 7. **FAQ Section**

**Location**: Lines 470-580 (approximately)

Each FAQ item has:
- A question (in the button)
- An answer (in the hidden section)

**Current structure:**
```html
<button class="faq-question w-full px-6 py-5 flex items-center justify-between hover:bg-gray-50 transition-colors duration-300 cursor-pointer">
    <span class="text-lg heading-primary text-[#1A1A1A] text-left">
        What is the time commitment required for the academy?
    </span>
    <!-- Icon code - don't modify -->
</button>
<div class="faq-answer hidden border-t border-gray-200 px-6 py-5 text-light text-gray-600">
    <p>Most participants dedicate 5-8 hours per week...</p>
</div>
```

**To update FAQ questions and answers:**
1. Find: `What is the time commitment required for the academy?`
2. Replace with your question
3. Find: `Most participants dedicate 5-8 hours...`
4. Replace with your answer

**Note**: You can have as many FAQ items as you want. To add a new FAQ:
1. Copy the entire FAQ item block (from `<div class="faq-item">` to `</div>`)
2. Paste it below the last FAQ item
3. Update the question and answer text

---

#### 8. **CTA Section (Call-to-Action)**

**Location**: Lines 600-620 (approximately)

```html
<h2 class="text-4xl md:text-5xl heading-primary text-white mb-6">
    Ready to Transform Your Leadership?
</h2>
<p class="text-xl text-light text-gray-200 mb-8">
    Join hundreds of leaders who have already discovered their purpose and influence. Your journey to exceptional leadership starts today.
</p>
```

**To update this section:**
1. Find: `Ready to Transform Your Leadership?` → Replace with your CTA headline
2. Find: `Join hundreds of leaders...` → Replace with your CTA message

---

#### 9. **Footer**

**Location**: Lines 680-750 (approximately)

Footer contains:
- Company tagline
- Quick links
- Resources
- Social media links
- Copyright information

**To update footer text:**
1. Find: `Transforming leaders, empowering organizations, changing the world.` → Replace with your tagline
2. Find: `© 2025 Leadership Academy. All rights reserved.` → Update year and company name
3. Find: `Empowering leaders worldwide` → Replace with your footer message

---

### Updating the Contact Email

**Location**: Multiple places

Your email address appears in:
1. Footer (line ~740)
2. Contact section (line ~620)
3. About page link (line ~620)

**To update your email everywhere:**
1. Use Find & Replace (`Ctrl+H`)
2. Find: `leaddershipacademy@leaddership.co.za`
3. Replace with: `your-email@yourdomain.com`
4. Click "Replace All"

---

## Modifying Styles with Tailwind CSS

### What is Tailwind CSS?

Tailwind CSS is a system of pre-made classes that control how your page looks. Instead of writing custom CSS, you add class names to HTML elements.

### Understanding Tailwind Classes

Tailwind classes are descriptive and follow patterns:

```
Padding:           p-4 (padding all sides), px-6 (horizontal), py-8 (vertical)
Margin:            m-4 (margin all sides), mb-6 (margin-bottom)
Text Size:         text-sm, text-lg, text-2xl, text-4xl, text-5xl
Text Weight:       font-light, font-semibold, font-bold
Background Color:  bg-white, bg-gray-50, bg-[#FF5A5F]
Text Color:        text-white, text-gray-600, text-[#1A1A1A]
Display:           flex, grid, hidden
Width/Height:      w-10, h-10, w-full, h-screen
Rounded Corners:   rounded-lg, rounded-full
Shadow:            shadow-md, shadow-lg
Responsive:        md:text-6xl (medium screens), lg:px-8 (large screens)
```

### Common Style Changes

#### Change Button Color

**Current primary button:**
```html
<a href="https://leaddership.co.za/join" class="btn-outline text-center font-semibold">
    Start Your Journey
</a>
```

The `btn-outline` class is defined in the `<style>` section. To change the button color:

1. Find this in the `<style>` section (line ~35):
```css
.btn-outline {
    background: transparent;
    border: 2px solid #FF5A5F;
    color: #FF5A5F;
    ...
}

.btn-outline:hover {
    background: #FF5A5F;
    ...
}
```

2. Replace `#FF5A5F` with your desired color:
   - For blue: `#0066CC`
   - For green: `#00AA44`
   - For purple: `#7C3AED`

**Example - Change to blue:**
```css
.btn-outline {
    background: transparent;
    border: 2px solid #0066CC;
    color: #0066CC;
    ...
}

.btn-outline:hover {
    background: #0066CC;
    ...
}
```

---

#### Change Text Size

**To make heading text larger:**

Find the heading you want to change. For example, the main hero heading:
```html
<h1 class="text-5xl md:text-6xl lg:text-7xl heading-primary text-[#1A1A1A] leading-tight mb-6">
```

The size classes work like this:
- `text-5xl` - Size on small screens (phones)
- `md:text-6xl` - Size on medium screens (tablets)
- `lg:text-7xl` - Size on large screens (desktops)

**To make it bigger:**
- Change `text-5xl` to `text-6xl`
- Change `md:text-6xl` to `md:text-7xl`
- Change `lg:text-7xl` to `lg:text-8xl`

**Result:**
```html
<h1 class="text-6xl md:text-7xl lg:text-8xl heading-primary text-[#1A1A1A] leading-tight mb-6">
```

---

#### Change Section Background Color

**Current features section:**
```html
<section id="features" class="py-20 md:py-28 px-4 sm:px-6 lg:px-8 bg-gray-50">
```

The `bg-gray-50` controls the background. To change it:

- `bg-white` - White background
- `bg-gray-50` - Light gray (current)
- `bg-gray-100` - Medium gray
- `bg-[#F0F7FF]` - Light blue

**Example - Change to white:**
```html
<section id="features" class="py-20 md:py-28 px-4 sm:px-6 lg:px-8 bg-white">
```

---

#### Add Spacing Between Elements

The `mb-` (margin-bottom) and `mt-` (margin-top) classes control spacing:

- `mb-2` - Small space
- `mb-4` - Medium space
- `mb-6` - Larger space
- `mb-8` - Even larger space
- `mb-12` - Large space
- `mb-16` - Very large space

**Example - Add more space between hero and features:**

Find:
```html
</section>

<!-- Features Section -->
<section id="features" class="py-20 md:py-28 px-4 sm:px-6 lg:px-8 bg-gray-50">
```

Change to:
```html
</section>

<!-- Features Section -->
<section id="features" class="py-20 md:py-28 px-4 sm:px-6 lg:px-8 bg-gray-50 mt-12">
```

---

#### Adjust Padding Inside Cards

**Current feature card:**
```html
<div class="card-hover bg-white p-8 shadow-md">
```

The `p-8` controls padding on all sides. Options:
- `p-4` - Tight padding
- `p-6` - Medium padding
- `p-8` - Current padding
- `p-10` - Loose padding

**To make cards less crowded:**
```html
<div class="card-hover bg-white p-10 shadow-md">
```

---

#### Change Shadow Effect

Shadows control the depth effect:
- `shadow-sm` - Subtle shadow
- `shadow-md` - Medium shadow (current)
- `shadow-lg` - Large shadow
- `shadow-xl` - Extra large shadow

**To add more depth to cards:**

Find:
```html
<div class="card-hover bg-white p-8 shadow-md">
```

Change to:
```html
<div class="card-hover bg-white p-8 shadow-lg">
```

---

#### Change Text Color

**Current body text:**
```html
<p class="text-light text-gray-600">
```

The `text-gray-600` controls color. Options:
- `text-gray-400` - Light gray (for secondary text)
- `text-gray-600` - Medium gray (current)
- `text-gray-800` - Dark gray
- `text-[#1A1A1A]` - Very dark (almost black)
- `text-[#FF5A5F]` - Red (accent color)

**Example - Make text darker for better readability:**
```html
<p class="text-light text-gray-700">
```

---

### Responsive Design (Mobile, Tablet, Desktop)

Your page automatically adjusts for different screen sizes. The prefixes mean:

- **No prefix** (e.g., `text-5xl`) - Applies to all screen sizes
- **`sm:`** - Small screens (640px and up)
- **`md:`** - Medium screens/tablets (768px and up)
- **`lg:`** - Large screens/desktops (1024px and up)
- **`xl:`** - Extra large screens (1280px and up)

**Example - Hero heading:**
```html
<h1 class="text-5xl md:text-6xl lg:text-7xl heading-primary text-[#1A1A1A]">
```

This means:
- On phones: `text-5xl` (large)
- On tablets: `md:text-6xl` (larger)
- On desktops: `lg:text-7xl` (largest)

**To adjust mobile appearance:**
Change the first class (no prefix):
```html
<h1 class="text-4xl md:text-6xl lg:text-7xl heading-primary text-[#1A1A1A]">
```

---

### Changing Icon Colors

Icons are SVG elements. To change their color:

**Current icon in features:**
```html
<svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24" stroke-width="1.5">
```

The `text-white` controls the color. Change it to:
- `text-white` - White
- `text-[#FF5A5F]` - Red
- `text-gray-600` - Gray

**Example - Change to red:**
```html
<svg class="w-6 h-6 text-[#FF5A5F]" fill="none" stroke="currentColor" viewBox="0 0 24 24" stroke-width="1.5">
```

---

## Fixing and Managing Links

### Understanding Links in Your Page

Links appear in several places:

1. **Navigation menu** (header)
2. **Buttons** (CTAs - Call-to-Action)
3. **Footer links**
4. **Internal anchor links** (jump to sections)

### Current Links in Your Page

#### Navigation Links (Header)

**Location**: Lines 72-86 (desktop menu) and 89-97 (mobile menu)

```html
<!-- Desktop Navigation -->
<a href="#features" class="text-[#1A1A1A] font-light hover:text-[#FF5A5F] transition-colors duration-300">Features</a>
<a href="#benefits" class="text-[#1A1A1A] font-light hover:text-[#FF5A5F] transition-colors duration-300">Benefits</a>
<a href="#testimonials" class="text-[#1A1A1A] font-light hover:text-[#FF5A5F] transition-colors duration-300">Testimonials</a>
<a href="#faq" class="text-[#1A1A1A] font-light hover:text-[#FF5A5F] transition-colors duration-300">FAQ</a>
<a href="https://leaddership.co.za/join" class="btn-outline">Join Now</a>
```

**What these links do:**
- `href="#features"` - Jumps to the Features section on the same page
- `href="#benefits"` - Jumps to the Benefits section
- `href="#testimonials"` - Jumps to the Testimonials section
- `href="#faq"` - Jumps to the FAQ section
- `href="https://leaddership.co.za/join"` - Goes to external website

---

#### CTA Buttons

**Location**: Throughout the page (hero, benefits, CTA section)

```html
<a href="https://leaddership.co.za/join" class="btn-outline text-center font-semibold">
    Start Your Journey
</a>
```

These buttons currently link to `https://leaddership.co.za/join`. You'll need to update this to your actual signup page.

---

#### Footer Links

**Location**: Lines 710-735 (approximately)

```html
<!-- Quick Links -->
<a href="#features" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Features</a>
<a href="#benefits" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Benefits</a>
<a href="#testimonials" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Testimonials</a>
<a href="#faq" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">FAQ</a>

<!-- Resources -->
<a href="blog.html" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Blog</a>
<a href="privacy.html" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Privacy Policy</a>
<a href="terms.html" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Terms of Service</a>
<a href="mailto:leaddershipacademy@leaddership.co.za" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Contact Us</a>

<!-- Social Media -->
<a href="#" class="w-10 h-10 bg-gray-700 rounded-lg flex items-center justify-center hover:bg-[#FF5A5F] transition-colors duration-300" aria-label="LinkedIn">
    <i class="fab fa-linkedin-in text-white"></i>
</a>
```

---

### Step-by-Step: Updating Links

#### Step 1: Update the Main "Join Now" Button

**Current:**
```html
<a href="https://leaddership.co.za/join" class="btn-outline">Join Now</a>
```

**To update:**
1. Find: `href="https://leaddership.co.za/join"`
2. Replace with: `href="https://your-domain.com/signup"` (your actual signup page)

**Example:**
```html
<a href="https://myacademy.com/enroll" class="btn-outline">Join Now</a>
```

---

#### Step 2: Update All CTA Buttons

Use Find & Replace to update all instances:

1. Press `Ctrl+H` to open Find & Replace
2. Find: `https://leaddership.co.za/join`
3. Replace with: `https://your-domain.com/signup`
4. Click "Replace All"

This updates all buttons throughout the page.

---

#### Step 3: Update Email Links

**Current:**
```html
<a href="mailto:leaddershipacademy@leaddership.co.za">leaddershipacademy@leaddership.co.za</a>
```

**To update:**
1. Find: `leaddershipacademy@leaddership.co.za`
2. Replace with: `your-email@yourdomain.com`

**Note**: This appears multiple times, so use "Replace All"

---

#### Step 4: Update Social Media Links

**Current social links in footer (lines 728-745):**
```html
<a href="#" class="w-10 h-10 bg-gray-700 rounded-lg flex items-center justify-center hover:bg-[#FF5A5F]" aria-label="LinkedIn">
    <i class="fab fa-linkedin-in text-white"></i>
</a>
```

**To update:**
1. Find: `href="#"` (for each social link)
2. Replace with your actual social media URL

**Examples:**
```html
<!-- LinkedIn -->
<a href="https://www.linkedin.com/company/your-company" class="w-10 h-10 bg-gray-700 rounded-lg flex items-center justify-center hover:bg-[#FF5A5F]" aria-label="LinkedIn">
    <i class="fab fa-linkedin-in text-white"></i>
</a>

<!-- Twitter -->
<a href="https://twitter.com/your-handle" class="w-10 h-10 bg-gray-700 rounded-lg flex items-center justify-center hover:bg-[#FF5A5F]" aria-label="Twitter">
    <i class="fab fa-twitter text-white"></i>
</a>

<!-- Facebook -->
<a href="https://www.facebook.com/your-page" class="w-10 h-10 bg-gray-700 rounded-lg flex items-center justify-center hover:bg-[#FF5A5F]" aria-label="Facebook">
    <i class="fab fa-facebook-f text-white"></i>
</a>

<!-- Instagram -->
<a href="https://www.instagram.com/your-handle" class="w-10 h-10 bg-gray-700 rounded-lg flex items-center justify-center hover:bg-[#FF5A5F]" aria-label="Instagram">
    <i class="fab fa-instagram text-white"></i>
</a>
```

---

#### Step 5: Add Links to Blog (Optional)

The footer currently has a link to `blog.html`:
```html
<a href="blog.html" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Blog</a>
```

If you don't have a blog page yet, you can:
- **Option A**: Remove this link
- **Option B**: Create a `blog.html` file
- **Option C**: Link to an external blog

**To remove the blog link:**
Find and delete this entire line:
```html
<a href="blog.html" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Blog</a>
```

---

### Common Link Issues and Fixes

#### Issue: Links Don't Work

**Possible causes:**
1. **Wrong URL format**: Make sure external URLs start with `https://` or `http://`
2. **File not found**: If linking to a local file (like `privacy.html`), make sure the file exists in the same folder
3. **Typo in anchor**: If using `#section-name`, make sure a matching `id="section-name"` exists

**Fix:**
- External links should look like: `href="https://example.com"`
- Internal links should look like: `href="#section-id"`
- Local files should look like: `href="page.html"`

---

#### Issue: Anchor Links Don't Scroll Smoothly

Your page has smooth scrolling built in (see JavaScript at the bottom). If it's not working:

1. Make sure the section has an `id` attribute:
```html
<section id="features" class="...">
```

2. Make sure the link uses the matching `id`:
```html
<a href="#features">Go to Features</a>
```

3. Check that there are no typos in the `id` or `href`

---

#### Issue: External Links Open in Same Tab

By default, links open in the same tab. To open in a new tab:

**Current:**
```html
<a href="https://example.com">External Link</a>
```

**To open in new tab:**
```html
<a href="https://example.com" target="_blank">External Link</a>
```

The `target="_blank"` attribute makes links open in a new tab.

---

## Adding Privacy and Terms Pages

### Why You Need These Pages

Privacy and Terms pages are important for:
- Legal compliance
- Building user trust
- Protecting your business
- Meeting website requirements

### Creating the Privacy Policy Page

#### Step 1: Create a New File

1. Open a text editor (VS Code, Notepad++, or Notepad)
2. Create a new file
3. Save it as `privacy.html` in the same folder as your `index.html`

#### Step 2: Add the Basic HTML Structure

Copy and paste this template into your `privacy.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy - Leadership Academy">
    <title>Privacy Policy | Leadership Academy</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            font-family: 'Inter', sans-serif;
        }
        h1, h2, h3, h4, h5, h6 {
            font-family: 'Space Grotesk', sans-serif;
        }
    </style>
</head>
<body class="bg-white">
    <!-- Header -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <div class="w-10 h-10 bg-gradient-to-br from-[#FF5A5F] to-[#FFD166] rounded-lg flex items-center justify-center">
                    <span class="text-white font-bold text-lg">LA</span>
                </div>
                <span class="text-xl font-bold text-[#1A1A1A]">Leadership</span>
            </div>
            <a href="index.html" class="text-[#1A1A1A] font-light hover:text-[#FF5A5F] transition-colors duration-300">Back to Home</a>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-20 md:py-28 px-4 sm:px-6 lg:px-8">
        <div class="max-w-4xl mx-auto">
            <h1 class="text-4xl md:text-5xl font-bold text-[#1A1A1A] mb-8">Privacy Policy</h1>
            
            <div class="prose prose-lg max-w-none">
                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">1. Introduction</h2>
                <p class="text-gray-600 mb-6">
                    Leadership Academy ("we," "us," "our," or "Company") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you visit our website.
                </p>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">2. Information We Collect</h2>
                <p class="text-gray-600 mb-4">We may collect information about you in a variety of ways. The information we may collect on the Site includes:</p>
                <ul class="list-disc list-inside text-gray-600 mb-6 space-y-2">
                    <li><strong>Personal Data:</strong> Name, email address, phone number, mailing address, and other contact information you voluntarily provide.</li>
                    <li><strong>Payment Information:</strong> Credit card and billing information (processed securely through third-party payment processors).</li>
                    <li><strong>Usage Data:</strong> Information about how you interact with our website, including pages visited, time spent, and clickstream data.</li>
                    <li><strong>Device Information:</strong> Information about your device, browser type, IP address, and operating system.</li>
                </ul>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">3. How We Use Your Information</h2>
                <p class="text-gray-600 mb-4">We use the information we collect for various purposes:</p>
                <ul class="list-disc list-inside text-gray-600 mb-6 space-y-2">
                    <li>To provide, maintain, and improve our services</li>
                    <li>To process transactions and send related information</li>
                    <li>To send promotional communications (with your consent)</li>
                    <li>To respond to your inquiries and customer service requests</li>
                    <li>To analyze usage patterns and improve user experience</li>
                    <li>To comply with legal obligations</li>
                </ul>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">4. Data Security</h2>
                <p class="text-gray-600 mb-6">
                    We implement appropriate technical and organizational measures to protect your personal data against unauthorized access, alteration, disclosure, or destruction. However, no method of transmission over the Internet or electronic storage is 100% secure.
                </p>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">5. Third-Party Disclosure</h2>
                <p class="text-gray-600 mb-6">
                    We do not sell, trade, or rent your personal information to third parties. We may share information with service providers who assist us in operating our website and conducting our business, subject to confidentiality agreements.
                </p>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">6. Your Rights</h2>
                <p class="text-gray-600 mb-4">You have the right to:</p>
                <ul class="list-disc list-inside text-gray-600 mb-6 space-y-2">
                    <li>Access your personal data</li>
                    <li>Correct inaccurate data</li>
                    <li>Request deletion of your data</li>
                    <li>Opt-out of marketing communications</li>
                    <li>Data portability</li>
                </ul>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">7. Cookies</h2>
                <p class="text-gray-600 mb-6">
                    Our website uses cookies to enhance your experience. You can choose to disable cookies through your browser settings, though this may affect site functionality.
                </p>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">8. Contact Us</h2>
                <p class="text-gray-600 mb-6">
                    If you have questions about this Privacy Policy or our privacy practices, please contact us at:
                </p>
                <p class="text-gray-600 mb-6">
                    <strong>Email:</strong> <a href="mailto:leaddershipacademy@leaddership.co.za" class="text-[#FF5A5F] hover:text-[#FFD166]">leaddershipacademy@leaddership.co.za</a><br>
                    <strong>Last Updated:</strong> 2025
                </p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-[#1A1A1A] text-white py-8 px-4 sm:px-6 lg:px-8">
        <div class="max-w-7xl mx-auto text-center">
            <p class="text-light text-gray-400">
                &copy; 2025 Leadership Academy. All rights reserved.
            </p>
            <div class="mt-4 space-x-4">
                <a href="index.html" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Home</a>
                <a href="privacy.html" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Privacy</a>
                <a href="terms.html" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Terms</a>
            </div>
        </div>
    </footer>
</body>
</html>
```

#### Step 3: Customize the Privacy Policy

Replace the placeholder content with your actual privacy policy:

1. Find: `Leadership Academy ("we," "us," "our," or "Company")`
2. Replace with your company name

3. Update the email address:
   - Find: `leaddershipacademy@leaddership.co.za`
   - Replace with your email

4. Update the "Last Updated" date:
   - Find: `<strong>Last Updated:</strong> 2025`
   - Replace with today's date

5. Customize each section with your actual policies

---

### Creating the Terms of Service Page

#### Step 1: Create a New File

1. Open a text editor
2. Create a new file
3. Save it as `terms.html` in the same folder as your `index.html`

#### Step 2: Add the Basic HTML Structure

Copy and paste this template into your `terms.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service - Leadership Academy">
    <title>Terms of Service | Leadership Academy</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            font-family: 'Inter', sans-serif;
        }
        h1, h2, h3, h4, h5, h6 {
            font-family: 'Space Grotesk', sans-serif;
        }
    </style>
</head>
<body class="bg-white">
    <!-- Header -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <div class="w-10 h-10 bg-gradient-to-br from-[#FF5A5F] to-[#FFD166] rounded-lg flex items-center justify-center">
                    <span class="text-white font-bold text-lg">LA</span>
                </div>
                <span class="text-xl font-bold text-[#1A1A1A]">Leadership</span>
            </div>
            <a href="index.html" class="text-[#1A1A1A] font-light hover:text-[#FF5A5F] transition-colors duration-300">Back to Home</a>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-20 md:py-28 px-4 sm:px-6 lg:px-8">
        <div class="max-w-4xl mx-auto">
            <h1 class="text-4xl md:text-5xl font-bold text-[#1A1A1A] mb-8">Terms of Service</h1>
            
            <div class="prose prose-lg max-w-none">
                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">1. Agreement to Terms</h2>
                <p class="text-gray-600 mb-6">
                    By accessing and using this website, you accept and agree to be bound by the terms and provision of this agreement. If you do not agree to abide by the above, please do not use this service.
                </p>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">2. Use License</h2>
                <p class="text-gray-600 mb-4">
                    Permission is granted to temporarily download one copy of the materials (information or software) on Leadership Academy's website for personal, non-commercial transitory viewing only. This is the grant of a license, not a transfer of title, and under this license you may not:
                </p>
                <ul class="list-disc list-inside text-gray-600 mb-6 space-y-2">
                    <li>Modifying or copying the materials</li>
                    <li>Using the materials for any commercial purpose or for any public display</li>
                    <li>Attempting to decompile or reverse engineer any software contained on the website</li>
                    <li>Removing any copyright or other proprietary notations from the materials</li>
                    <li>Transferring the materials to another person or "mirroring" the materials on any other server</li>
                </ul>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">3. Disclaimer</h2>
                <p class="text-gray-600 mb-6">
                    The materials on Leadership Academy's website are provided on an 'as is' basis. Leadership Academy makes no warranties, expressed or implied, and hereby disclaims and negates all other warranties including, without limitation, implied warranties or conditions of merchantability, fitness for a particular purpose, or non-infringement of intellectual property or other violation of rights.
                </p>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">4. Limitations</h2>
                <p class="text-gray-600 mb-6">
                    In no event shall Leadership Academy or its suppliers be liable for any damages (including, without limitation, damages for loss of data or profit, or due to business interruption) arising out of the use or inability to use the materials on Leadership Academy's website, even if Leadership Academy or an authorized representative has been notified orally or in writing of the possibility of such damage.
                </p>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">5. Accuracy of Materials</h2>
                <p class="text-gray-600 mb-6">
                    The materials appearing on Leadership Academy's website could include technical, typographical, or photographic errors. Leadership Academy does not warrant that any of the materials on its website are accurate, complete, or current. Leadership Academy may make changes to the materials contained on its website at any time without notice.
                </p>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">6. Links</h2>
                <p class="text-gray-600 mb-6">
                    Leadership Academy has not reviewed all of the sites linked to its website and is not responsible for the contents of any such linked site. The inclusion of any link does not imply endorsement by Leadership Academy of the site. Use of any such linked website is at the user's own risk.
                </p>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">7. Modifications</h2>
                <p class="text-gray-600 mb-6">
                    Leadership Academy may revise these terms of service for its website at any time without notice. By using this website, you are agreeing to be bound by the then current version of these terms of service.
                </p>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">8. Governing Law</h2>
                <p class="text-gray-600 mb-6">
                    These terms and conditions are governed by and construed in accordance with the laws of [Your Jurisdiction], and you irrevocably submit to the exclusive jurisdiction of the courts in that location.
                </p>

                <h2 class="text-2xl font-bold text-[#1A1A1A] mt-8 mb-4">9. Contact Information</h2>
                <p class="text-gray-600 mb-6">
                    If you have any questions about these Terms of Service, please contact us at:
                </p>
                <p class="text-gray-600 mb-6">
                    <strong>Email:</strong> <a href="mailto:leaddershipacademy@leaddership.co.za" class="text-[#FF5A5F] hover:text-[#FFD166]">leaddershipacademy@leaddership.co.za</a><br>
                    <strong>Last Updated:</strong> 2025
                </p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-[#1A1A1A] text-white py-8 px-4 sm:px-6 lg:px-8">
        <div class="max-w-7xl mx-auto text-center">
            <p class="text-light text-gray-400">
                &copy; 2025 Leadership Academy. All rights reserved.
            </p>
            <div class="mt-4 space-x-4">
                <a href="index.html" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Home</a>
                <a href="privacy.html" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Privacy</a>
                <a href="terms.html" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Terms</a>
            </div>
        </div>
    </footer>
</body>
</html>
```

#### Step 3: Customize the Terms of Service

1. Replace `[Your Jurisdiction]` with your actual jurisdiction (e.g., "South Africa")
2. Update the email address with yours
3. Update the "Last Updated" date
4. Customize the terms with your specific policies

---

### Verifying Your Links Work

#### Test the Privacy and Terms Links

1. Save all three files (`index.html`, `privacy.html`, `terms.html`) in the same folder
2. Open `index.html` in your browser
3. Scroll to the footer
4. Click on "Privacy Policy" - it should go to `privacy.html`
5. Click on "Terms of Service" - it should go to `terms.html`
6. Click "Back to Home" to return to `index.html`

#### Common Issues:

**Issue**: Links don't work
- **Solution**: Make sure all three files are in the same folder

**Issue**: Page looks broken
- **Solution**: Make sure you saved the files with `.html` extension (not `.txt`)

**Issue**: Styling looks different
- **Solution**: This is normal - the pages use Tailwind CSS from CDN, which loads from the internet

---

### Updating Footer Links in index.html

Your footer already has the correct links to privacy.html and terms.html:

```html
<a href="privacy.html" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Privacy Policy</a>
<a href="terms.html" class="text-light text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Terms of Service</a>
```

These are already set up correctly and will work once you create the `privacy.html` and `terms.html` files.

---

## Common Customizations

### Adding a New Testimonial

#### Step 1: Find the Testimonials Section

**Location**: Lines 340-420

#### Step 2: Copy an Existing Testimonial

Find this block:
```html
<div class="card-hover bg-white p-6 shadow-md">
    <div class="flex items-center gap-1 mb-4">
        <!-- Stars -->
    </div>
    <p class="text-light text-gray-600 mb-4">
        "The Leadership Academy transformed..."
    </p>
    <div>
        <p class="font-semibold text-[#1A1A1A] heading-primary">Sarah Mitchell</p>
        <p class="text-sm text-light text-gray-500">Senior Manager, Tech Solutions Inc.</p>
    </div>
</div>
```

#### Step 3: Paste and Customize

Paste the block after the last testimonial and update:
- The testimonial quote
- The person's name
- Their title/company

---

### Adding a New FAQ Question

#### Step 1: Find the FAQ Section

**Location**: Lines 470-580

#### Step 2: Copy an Existing FAQ Item

Find this block:
```html
<div class="faq-item bg-white rounded-lg shadow-md overflow-hidden">
    <button class="faq-question w-full px-6 py-5 flex items-center justify-between hover:bg-gray-50 transition-colors duration-300 cursor-pointer">
        <span class="text-lg heading-primary text-[#1A1A1A] text-left">
            What is the time commitment required for the academy?
        </span>
        <!-- Icon -->
    </button>
    <div class="faq-answer hidden border-t border-gray-200 px-6 py-5 text-light text-gray-600">
        <p>Most participants dedicate 5-8 hours per week...</p>
    </div>
</div>
```

#### Step 3: Paste and Customize

Paste the block after the last FAQ item and update:
- The question text
- The answer text

---

### Changing the Color Scheme

#### Locate the Color Definitions

In the `<style>` section (lines 25-70), find:

```css
.btn-outline {
    border: 2px solid #FF5A5F;
    color: #FF5A5F;
}

.btn-outline:hover {
    background: #FF5A5F;
}
```

#### Replace with New Colors

**Example - Change from Red/Yellow to Blue/Purple:**

1. Find: `#FF5A5F` (red)
2. Replace with: `#0066CC` (blue)

3. Find: `#FFD166` (yellow)
4. Replace with: `#7C3AED` (purple)

---

### Adding a New Section

#### Basic Template

```html
<section class="py-20 md:py-28 px-4 sm:px-6 lg:px-8 bg-white">
    <div class="max-w-7xl mx-auto">
        <h2 class="text-4xl md:text-5xl heading-primary text-[#1A1A1A] mb-12 text-center">
            Your Section Title
        </h2>
        
        <p class="text-lg text-light text-gray-600 text-center mb-12">
            Your section description goes here.
        </p>
        
        <!-- Your content here -->
    </div>
</section>
```

#### Where to Add It

Add new sections between existing sections. For example, to add a section after Features:

1. Find: `</section>` after the Features section
2. Add your new section code right after it

---

### Changing Button Text

**Current button:**
```html
<a href="https://leaddership.co.za/join" class="btn-outline text-center font-semibold">
    Start Your Journey
</a>
```

**To change:**
1. Find: `Start Your Journey`
2. Replace with: `Your New Button Text`

---

### Adding an Image

To add an image to your page:

```html
<img src="path/to/image.jpg" alt="Description of image" class="w-full rounded-lg shadow-md">
```

**Where to put images:**
- Create a folder called `images` in the same location as your HTML files
- Save images in that folder
- Use: `src="images/my-image.jpg"`

---

### Hiding Elements

To hide an element without deleting it:

Find the element and add the `hidden` class:

```html
<!-- Before -->
<div class="card-hover bg-white p-8 shadow-md">
    ...
</div>

<!-- After (hidden) -->
<div class="card-hover bg-white p-8 shadow-md hidden">
    ...
</div>
```

---

## Troubleshooting

### Common Problems and Solutions

#### Problem: Page Looks Broken or Unstyled

**Causes:**
1. Tailwind CSS CDN is not loading
2. Browser cache is outdated
3. Missing `<style>` section

**Solutions:**
1. Clear browser cache (Ctrl+Shift+Delete)
2. Try a different browser
3. Check internet connection (Tailwind loads from CDN)
4. Hard refresh (Ctrl+Shift+R)

---

#### Problem: Links Don't Work

**Causes:**
1. Typo in URL
2. Missing `https://` for external links
3. File doesn't exist in the same folder

**Solutions:**
1. Double-check the URL spelling
2. Make sure external URLs start with `https://`
3. Make sure local files (privacy.html, terms.html) are in the same folder
4. Use Find & Replace to check for typos

---

#### Problem: Text Appears Too Small or Too Large

**Causes:**
1. Wrong Tailwind size class
2. Browser zoom level

**Solutions:**
1. Check the text size class:
   - `text-sm` = small
   - `text-lg` = large
   - `text-2xl` = extra large
   - `text-5xl` = very large
2. Reset browser zoom (Ctrl+0)

---

#### Problem: Colors Look Wrong

**Causes:**
1. Wrong color code in style section
2. Color code format error

**Solutions:**
1. Verify color codes are in correct format: `#RRGGBB`
2. Check for typos in hex codes
3. Use a color picker tool to verify colors

---

#### Problem: Mobile Menu Doesn't Work

**Causes:**
1. JavaScript is disabled
2. Mobile menu code is deleted
3. Browser compatibility issue

**Solutions:**
1. Check if JavaScript is enabled in browser settings
2. Verify mobile menu code is intact (lines 89-97)
3. Try a different browser

---

#### Problem: Contact Form Doesn't Send

**Causes:**
1. Web3Forms access key is invalid
2. Internet connection issue
3. Browser security settings

**Solutions:**
1. Verify the Web3Forms access key is correct
2. Check internet connection
3. Try a different browser
4. Check browser console for error messages (F12)

---

### Getting Help with HTML/CSS

#### Useful Resources:

- **HTML Reference**: https://developer.mozilla.org/en-US/docs/Web/HTML
- **CSS Reference**: https://developer.mozilla.org/en-US/docs/Web/CSS
- **Tailwind CSS Docs**: https://tailwindcss.com/docs
- **Color Picker**: https://www.w3schools.com/colors/colors_picker.asp
- **Font Awesome Icons**: https://fontawesome.com/icons

#### Debugging Steps:

1. **Check the browser console** (Press F12)
   - Look for error messages in red
   - Errors often tell you exactly what's wrong

2. **Use browser inspector** (Right-click → Inspect)
   - Click on elements to see their HTML and CSS
   - Modify CSS in real-time to test changes

3. **Validate your HTML** (https://validator.w3.org/)
   - Copy your HTML code
   - Paste into validator
   - It will show any errors

---

## Best Practices

### Maintenance Best Practices

#### 1. **Keep Backups**
- Always keep a backup of your original `index.html`
- Before making major changes, save a copy as `index-backup.html`

#### 2. **Use Find & Replace Carefully**
- Always review replacements before clicking "Replace All"
- Make a backup first

#### 3. **Test Changes**
- After making changes, refresh your browser (Ctrl+F5)
- Test on mobile devices
- Test all links

#### 4. **Use Version Control (Optional)**
- Consider using GitHub to track changes
- This allows you to revert if something goes wrong

---

### Customization Best Practices

#### 1. **Keep Consistent Spacing**
- Use the same margin/padding values throughout
- Use: `mb-4`, `mb-6`, `mb-8` (not random values)

#### 2. **Keep Consistent Colors**
- Stick to your color scheme
- Don't add too many new colors
- Use the primary red and yellow as accents

#### 3. **Keep Consistent Typography**
- Use heading classes for headings
- Use body text classes for paragraphs
- Don't mix font sizes randomly

#### 4. **Mobile-First Approach**
- Always test on mobile devices
- Ensure responsive design works
- Check that navigation works on mobile

#### 5. **Accessibility**
- Add descriptive alt text to images
- Use semantic HTML (headings, paragraphs, etc.)
- Ensure sufficient color contrast

---

### Performance Best Practices

#### 1. **Optimize Images**
- Use compressed images
- Use appropriate image formats (JPG for photos, PNG for graphics)
- Specify image dimensions

#### 2. **Minimize External Requests**
- Limit third-party scripts
- Consider self-hosting fonts if using many

#### 3. **Test Page Speed**
- Use Google PageSpeed Insights
- Check Core Web Vitals
- Optimize for mobile speed

---

### Security Best Practices

#### 1. **Protect Your Contact Form**
- The Web3Forms integration is already secure
- Don't expose your email publicly in HTML comments

#### 2. **Use HTTPS**
- Always use `https://` for external links
- Ensure your website uses HTTPS

#### 3. **Keep Content Updated**
- Update testimonials and content regularly
- Remove outdated information
- Keep privacy/terms pages current

#### 4. **Validate User Input**
- The contact form already validates input
- Don't trust unvalidated user data

---

### SEO Best Practices

#### 1. **Meta Tags**
Your page already has good meta tags:
```html
<meta name="description" content="Lead With Purpose and Influence - Transform Your Skills...">
<meta name="keywords" content="leadership, professional development, online learning, personal growth">
```

Update these for better SEO:
- Keep description under 160 characters
- Include relevant keywords
- Make it compelling

#### 2. **Headings**
- Use H1 for main title (only one per page)
- Use H2 for section titles
- Use H3 for subsections
- Don't skip heading levels

#### 3. **Links**
- Use descriptive link text (not "click here")
- Add alt text to images
- Use internal links to connect related pages

#### 4. **Content**
- Write for humans first, search engines second
- Use natural language
- Include relevant keywords naturally
- Keep content updated

---

## Quick Reference

### File Structure

```
your-project-folder/
├── index.html          (Main landing page)
├── privacy.html        (Privacy policy)
├── terms.html          (Terms of service)
└── images/             (Optional: image folder)
    ├── logo.png
    └── hero-image.jpg
```

---

### Common Tailwind Classes

```
Spacing:
  p-4, p-6, p-8         (Padding)
  m-4, m-6, m-8         (Margin)
  mb-4, mt-4, mx-4      (Specific sides)

Text:
  text-sm, text-lg, text-2xl, text-4xl, text-5xl
  font-light, font-semibold, font-bold
  text-white, text-gray-600, text-[#FF5A5F]

Layout:
  flex, grid, hidden
  w-full, w-10, h-10
  rounded-lg, rounded-full

Responsive:
  md: (medium screens)
  lg: (large screens)
  sm: (small screens)

Effects:
  shadow-md, shadow-lg
  hover:text-[#FF5A5F]
  transition-colors duration-300
```

---

### Common Color Codes

```
Primary Red:      #FF5A5F
Primary Yellow:   #FFD166
Dark Text:        #1A1A1A
Light Gray:       #F3F4F6
Medium Gray:      #666666
White:            #FFFFFF
```

---

### Keyboard Shortcuts

```
Ctrl+H            Find & Replace
Ctrl+F            Find
Ctrl+S            Save
Ctrl+Z            Undo
Ctrl+Y            Redo
Ctrl+Shift+R      Hard refresh (clear cache)
F12               Open developer tools
```

---

## Final Checklist

Before launching your website:

- [ ] All text content is updated
- [ ] All links work correctly
- [ ] Email addresses are correct
- [ ] Contact form works
- [ ] Privacy and Terms pages are created and linked
- [ ] Social media links are updated
- [ ] Page looks good on mobile
- [ ] Page looks good on desktop
- [ ] All images load correctly
- [ ] No broken links
- [ ] No typos or grammatical errors
- [ ] Meta tags are updated
- [ ] Favicon is set (optional)
- [ ] Contact email is correct

---

## Support and Resources

### Need Help?

1. **Check this guide** - Most common issues are covered
2. **Browser console** - Press F12 and look for error messages
3. **HTML Validator** - https://validator.w3.org/
4. **Tailwind Docs** - https://tailwindcss.com/docs
5. **Stack Overflow** - Search for similar issues

### Next Steps

1. Customize all text content
2. Update all links
3. Create privacy and terms pages
4. Test everything
5. Deploy to web hosting
6. Monitor performance

---

## Conclusion

You now have a comprehensive guide to maintaining and customizing your Leadership Academy landing page. Remember:

- **Start small** - Make one change at a time
- **Test frequently** - Refresh your browser after each change
- **Keep backups** - Save copies before major changes
- **Stay consistent** - Follow the existing design patterns
- **Ask for help** - Don't hesitate to use the resources provided

Good luck with your leadership academy website! 🚀