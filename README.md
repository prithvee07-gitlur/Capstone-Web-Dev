# Capstone-Web-Dev
# FASHIONISTA - E-Commerce Capstone Project

[cite_start]**Project Name:** FASHIONISTA [cite: 1]  
[cite_start]**Author:** Prithvi [cite: 1]  
[cite_start]**Course:** Computer Science (B. Tech CSE) [cite: 1]  
**University:** K.R. [cite_start]Mangalam University [cite: 1, 2]  
[cite_start]**Date:** December 14, 2025 [cite: 2]

---

## 1. Project Overview
[cite_start]The objective of this assignment was to build a fully structured, responsive e-commerce web interface using HTML5 and CSS3[cite: 2]. [cite_start]"FASHIONISTA" is a landing page designed for a fashion e-commerce theme, allowing users to browse clothing collections, view flash sales, and read testimonials[cite: 3]. [cite_start]The design prioritizes a high-contrast visual hierarchy, ease of navigation, and clear calls to action[cite: 4].

## 2. Design Decisions & Visual Style

### Color Palette
[cite_start]A high-contrast monochrome scheme was utilized to create a modernistic, premium feel[cite: 5].
* [cite_start]**Primary Colors:** Black (`#222`) and White (`#fff`) for main UI elements and readability[cite: 6].
* [cite_start]**Accent Color:** Vibrant Red (`#ff4d4f`) for the "Flash Sale" banner and discount pricing to draw attention[cite: 7].

### Typography
* [cite_start]**Font Family:** "Montserrat" (imported from Google Fonts)[cite: 8].
* [cite_start]**Usage:** Used across the entire document to provide a geometric, modern look suitable for a fashion brand[cite: 9].

### Visual Effects
* [cite_start]**Sticky Navigation:** The navbar is set to `position: sticky` with a z-index and box-shadow to remain accessible during scrolling[cite: 10].
* [cite_start]**Hover States:** Product and category cards utilize `transform: scale` and increased box-shadows to create a "lifting" effect[cite: 11].
* [cite_start]**Image Overlays:** The Hero section uses a dark RGBA overlay (`rgba(0, 0, 0, 0.45)`) to ensure white text remains legible against background images[cite: 12].

## 3. Structural Implementation (HTML5)
[cite_start]Semantic HTML5 practices were followed to ensure a logical document flow[cite: 13]:
* [cite_start]**`<nav>`:** Contains the logotype, search bar, and user account links[cite: 13].
* [cite_start]**`<main>`:** Wraps primary content, separating the Sidebar and Main Section from the header and footer[cite: 14].
* [cite_start]**`<aside>`:** Used for the "Filters" sidebar (Category, Price, Color checkboxes)[cite: 15].
* [cite_start]**`<section>`:** Divides the page into thematic areas like the Hero Banner, Product Grid, and Testimonials[cite: 16].
* [cite_start]**`<footer>`:** Organized into a grid layout for links (Account, Help, Policies)[cite: 17].

## 4. Layout & Responsiveness
[cite_start]The layout adapts to different screen sizes using CSS Media Queries, Grid, and Flexbox[cite: 18].

### Grid & Flexbox Strategy
* [cite_start]**Grid Layouts:** Product and Best Seller grids use `grid-template-columns: repeat(auto-fit, minmax(220px, 1fr))` to allow automatic wrapping without specific breakpoints[cite: 18, 19].
* [cite_start]**Flexbox:** The main container uses Flexbox to align the Sidebar and Main Section side-by-side on desktop[cite: 20].

### Media Queries
* [cite_start]**Tablet (Max-width 1100px):** The flex direction switches to column, moving the Sidebar to the top of the content for better usability[cite: 21, 22].
* [cite_start]**Mobile (Max-width 768px):** Detailed navigation links are toggled off, and a Hamburger menu becomes visible to conserve space[cite: 23].

## 5. Challenges & Solutions

| Challenge | Solution |
| :--- | :--- |
| [cite_start]**Hero Text Readability:** Ensuring text was readable regardless of image brightness[cite: 28]. | [cite_start]Implemented a `.hero-overlay` div with a semi-transparent black background positioned behind the text[cite: 29]. |
| [cite_start]**Mobile Footer:** Making the footer look consistent on mobile vs. desktop[cite: 30]. | [cite_start]Utilized CSS Grid with `repeat(auto-fit, minmax(180px, 1fr))` to allow columns to stack automatically[cite: 31]. |
| [cite_start]**Sidebar on Small Screens:** Handling sidebar filters where horizontal space is limited[cite: 32]. | [cite_start]A media query at 1100px forces the sidebar to take 100% width, stacking it above products to maintain accessibility[cite: 33]. |

## 6. Key Learning Outcomes
Through developing this Capstone project, practical experience was gained in:
* [cite_start]**Advanced Positioning:** Using `position: sticky` for navigation[cite: 24].
* [cite_start]**Complex Layouts:** Combining fixed sidebars (`flex: 0 0 220px`) with fluid content areas (`flex: 1`)[cite: 25].
* [cite_start]**Styling Forms:** Customizing input fields (e.g., rounded search bars) to match brand identity[cite: 26].
* [cite_start]**Interactive Design:** implementing CSS transitions for responsive UI feedback[cite: 27].

---
[cite_start]*This project demonstrates a strong understanding of CSS Grid, Flexbox, and semantic HTML structure suitable for a modern web application[cite: 36].*
