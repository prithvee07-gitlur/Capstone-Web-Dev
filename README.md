# FASHIONISTA - E-Commerce Capstone Project

**Project Name:** FASHIONISTA  
**Author:** Prithvi  
**Course:** Computer Science (B. Tech CSE)  
**University:** K.R. Mangalam University  
**Date:** December 14, 2025

---

## 1. Project Overview
The objective of this assignment was to build a fully structured, responsive e-commerce web interface using HTML5 and CSS3. "FASHIONISTA" is a landing page designed for a fashion e-commerce theme, allowing users to browse clothing collections, view flash sales, and read testimonials. The design prioritizes a high-contrast visual hierarchy, ease of navigation, and clear calls to action.

## 2. Design Decisions & Visual Style

### Color Palette
A high-contrast monochrome scheme was utilized to create a modernistic, premium feel.
* **Primary Colors:** Black (`#222`) and White (`#fff`) are used for main UI elements to ensure text readability and a clean aesthetic.
* **Accent Color:** A vibrant Red (`#ff4d4f`) is used for the "Flash Sale" banner, discount pricing, and hover states to draw immediate user attention.

### Typography
* **Font Family:** "Montserrat" (imported from Google Fonts).
* **Usage:** Used across the entire document (body, headings) to provide a geometric, modern look suitable for a fashion brand.

### Visual Effects
* **Sticky Navigation:** The navbar is set to `position: sticky` with a z-index and box-shadow, ensuring it remains accessible as the user scrolls.
* **Hover States:** Interactive elements like product and category cards utilize `transform: scale` and increased box-shadows to create a "lifting" effect.
* **Image Overlays:** The Hero section utilizes a dark RGBA overlay (`rgba(0, 0, 0, 0.45)`) to ensure the white "Winter Sale" text remains legible against the busy background.

## 3. Structural Implementation (HTML5)
Semantic HTML5 practices were followed to ensure a logical document flow:
* **`<nav>`:** Contains the logotype, search bar, and user account links, serving as the primary navigation controller.
* **`<main>`:** Wraps the primary page content, including the Sidebar and the Main Section, separating it from the footer and header.
* **`<aside>`:** Used for the "Filters" sidebar, semantically indicating that this content (Category, Price, Color checkboxes) is related to but distinct from the main product grid.
* **`<section>`:** Divides the page into distinct thematic areas such as the Hero Banner, Product Grid, Best Sellers, and Testimonials.
* **`<footer>`:** Organized into a grid layout containing links for Account, Help, Policies, and social media.

## 4. Responsiveness Strategy
The layout adapts to different screen sizes using CSS Media Queries and flexible units:

### Grid & Flexbox
* **Grid Layouts:** The Product and Best Seller grids use `grid-template-columns: repeat(auto-fit, minmax(220px, 1fr))`. This ensures product cards automatically wrap and resize based on available width without requiring specific breakpoints.
* **Flexbox Layouts:** The main content container uses Flexbox. On desktop, it aligns the Sidebar and Main Section side-by-side.

### Media Queries
* **Tablet (Max-width 1100px):** The Flex direction of the main content switches to column, moving the Sidebar to the top of the content for better usability.
* **Mobile (Max-width 768px):** The detailed navigation links display is toggled off, and the Hamburger menu becomes visible to conserve screen space.

## 5. Challenges & Solutions

| Challenge | Solution |
| :--- | :--- |
| **Hero Text Readability:** Ensuring text on the Hero background was readable regardless of image brightness. | Implemented a `.hero-overlay` div with a semi-transparent black background positioned absolutely over the image but behind the text. |
| **Mobile Footer:** Making the Footer look consistent on mobile devices versus desktop. | Utilized CSS Grid for the footer with `repeat(auto-fit, minmax(180px, 1fr))`, allowing columns to stack automatically on smaller screens without complex floats. |
| **Sidebar on Small Screens:** Handling sidebar filters where horizontal space is limited. | A media query at 1100px forces the sidebar to take 100% width, effectively stacking it above the products to maintain accessibility. |

## 6. Learning Outcomes
Through the development of the "FASHIONISTA" Capstone project, practical experience was gained in:
* **Advanced Positioning:** Using `position: sticky` effectively for persistent navigation.
* **Complex Box Model & Layouts:** Combining `flex: 0 0 220px` for fixed sidebars and `flex: 1` for fluid content areas.
* **Styling Form Elements:** Styling input fields (e.g., rounded search bars with `border-radius: 20px`) to match brand identity.
* **Interactive Design:** Exploring CSS transitions (`transition: width 0.3s, transform 0.2s`) to make the UI feel responsive.
