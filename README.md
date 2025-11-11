# WEDE_BAKERY_POE_FINAL
# Sweet Savories Bakery Website 

This project represents the development of a website for **Sweet Savories Bakery**, an artisan bakery located in Pretoria. The website serves as an online presence for the bakery, showcasing their menu, allowing customers to place online orders, and providing essential information about the bakery’s services. This project was built as part of an assignment to practice front-end web development, focusing on HTML, CSS, and JavaScript.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features and Functionality](#features-and-functionality)
3. [Design Choices and Technical Implementation](#design-choices-and-technical-implementation)
4. [Challenges and Solutions](#challenges-and-solutions)
5. [File Structure](#file-structure)
6. [Future Improvements](#future-improvements)
7. [Conclusion](#conclusion)
8. [License](#license)
9. [Contact Information](#contact-information)

---

## Project Overview

The **Sweet Savories Bakery** website was designed to reflect the bakery's commitment to quality and freshly baked goods. It includes various interactive sections such as the homepage with an introductory overview, a menu page with product filtering, and an online ordering system that enables customers to view and add items to their cart.

The website was built using:
- **HTML** for structuring the content.
- **CSS** for styling the website and ensuring it’s visually appealing and responsive across devices.
- **JavaScript** for adding interactive features like filtering the menu and handling dynamic content updates.

### Key Features:
- **Responsive Design**: Mobile-friendly layout that adjusts to different screen sizes using CSS Flexbox and Grid.
- **Menu Filtering**: Users can filter menu items by categories (e.g., Bread, Cakes, Pastries, Savory).
- **Online Ordering**: Users can add items to their cart with a simple “Add to Order” button (backend integration for actual order processing can be added later).
- **SEO Optimized**: Search engine-friendly with well-structured metadata, alt attributes for images, and semantic HTML tags.
- **Accessibility**: Skip links, ARIA roles, and alt text for better navigation and support for screen readers.

---

## Features and Functionality

### 1. **Homepage Design**
The homepage serves as the introduction to the bakery. It features:
- A **hero section** with a prominent bakery image and a tagline ("Freshly baked goods made with love since 2010").
- **Call-to-action buttons** that direct users to the menu or order pages.
- **Navigation**: The navigation bar allows quick access to the main pages (Home, Menu, Order Online, Our Story, Contact).

The goal of the homepage is to make a strong first impression by showing high-quality images of the bakery’s products and a brief introduction. It’s crucial to evoke a sense of warmth and trust to encourage customers to explore the site further.

### 2. **Menu Page with Category Filters**
The **Menu page** displays all bakery items with a **filtering system** that allows users to sort by product categories such as **Bread**, **Cakes**, **Pastries**, and **Savory**.

Each item includes:
- An **image** showcasing the product.
- A **short description** of the item.
- A **price** tag for each product.
- An **Add to Order** button, which directs users to the order page.

**JavaScript** functionality is used to filter products by category, providing a smooth user experience.

**JavaScript code for filtering functionality:**
```javascript
// JavaScript for filtering menu items based on category
const filterButtons = document.querySelectorAll('.filter-btn');
const menuItems = document.querySelectorAll('.menu-item');

filterButtons.forEach(button => {
  button.addEventListener('click', () => {
    const filter = button.getAttribute('data-filter');
    
    // Highlight active button
    filterButtons.forEach(btn => btn.classList.remove('active'));
    button.classList.add('active');
    
    // Show/hide items based on category
    menuItems.forEach(item => {
      if (filter === 'all' || item.getAttribute('data-category') === filter) {
        item.style.display = 'block';
      } else {
        item.style.display = 'none';
      }
    });
  });
});
Refrences.
W3Schools, CSS Tutorial, Available at: https://www.w3schools.com/css/
 [Accessed 11 November 2025].

JavaScript.info, JavaScript Guide, Available at: https://javascript.info/
 [Accessed 11 November 2025].

Mozilla Developer Network (MDN), JavaScript Documentation, Available at: https://developer.mozilla.org/en-US/docs/Web/JavaScript
 [Accessed 11 November 2025].

Google Developers, Web Fundamentals: Lazy Loading Images, Available at: https://developers.google.com/web/fundamentals/performance/lazy-loading-guidance/images-and-video
 [Accessed 11 November 2025].

Google Chrome Developers, 2020. Lazy Loading Images for Faster Performance. Available at: https://www.youtube.com/watch?v=W42ykt-s0lg
 [Accessed 11 November 2025].

freeCodeCamp.org, 2020. Git and GitHub for Beginners - Crash Course. Available at: https://www.youtube.com/watch?v=RGOj5yH7evk
 [Accessed 11 November 2025].

Moz, 2021. SEO for Beginners - Learn SEO. Available at: https://www.youtube.com/watch?v=gm8IuEUB7ds
 [Accessed 11 November 2025].
