#📦 E-Commerce Product Filter System

A modern front-end web application that allows users to dynamically filter products based on categories, price range, ratings, search queries, and availability — all with real-time updates.

Designed as a responsive mini-project for showcasing UI/UX skills, JavaScript filtering logic, and client-side performance.

🚀 Project Overview

This project demonstrates how an e-commerce platform can provide instant, client-side product filtering without requiring page reloads or a backend.

Users can smoothly browse through products, apply multiple filters, and get immediate results thanks to JavaScript DOM manipulation and event-driven rendering.

✨ Key Features
🔍 1. Dynamic Category Filtering

Users can select product categories (Electronics, Fashion, Home, Sports, etc.) to instantly filter visible items.

💰 2. Price Range Slider

A smooth, real-time slider allows users to adjust the maximum price.
Products update instantly based on the selected price range.

⭐ 3. Rating Filter / Sorter

Products can be sorted by:

Featured

Price: Low → High

Price: High → Low

Highest Rated

📦 4. Availability Toggle

Enable In Stock Only to hide products that are currently unavailable.

📝 5. Search Functionality

Users can search products by:

Product name

Brand name

The results update as you type.

⚡ 6. Real-Time Results (No Reloads)

All filtering and sorting happens instantly using:

JavaScript arrays

Filter conditions

DOM rendering

No backend required.

🖥️ 7. Responsive Layout

Works seamlessly on:

Desktop

Tablet

Mobile

Built using Bootstrap 5 grid system.

❤️ 8. Wishlist Support (Optional)

Users can mark items as favorites using the heart icon.

🛒 9. Mini Floating Cart

Add items to cart and instantly view:

Item count

Subtotal

Quick remove options

🎨 10. Clean & Modern UI

Features include:

Soft gradients

Rounded cards

Minimalistic icons

Smooth hover effects

🔧 Technologies Used
Technology	Purpose
HTML5	Structure
CSS3	Styling, UI Design
Bootstrap 5	Layout, components, responsiveness
JavaScript (ES6)	Filtering, UI updates, cart/wishlist logic
Bootstrap Icons	Icons for UI elements
🧠 How Filtering Works (Logic Explained)

Product data is stored as an array of objects:

{
  id: 101,
  title: "iPhone 15 Pro Titanium",
  category: "Electronics",
  brand: "Apple",
  price: 134900,
  rating: 4.9,
  stock: true,
  sale: false
}


Filters include:

Search Filter

p.title.toLowerCase().includes(query)


Category Filter

p.category === selectedCategory


Price Range

p.price <= maxPrice


Stock Availability

inStockOnly ? p.stock === true : true


Sorting

list.sort((a, b) => a.price - b.price);


Finally, filtered results are rendered back to the DOM using:

document.getElementById('productArea').innerHTML = html;

🛠️ How to Run the Project

Download the project folder

Open index.html in any browser

No installation required—fully client-side

To add new products:
Open script.js, and push new items into productCatalog[]

📁 Folder Structure
project-folder/
 ├── index.html
 ├── script.js
 ├── styles.css (optional)
 ├── assets/ (images, icons)
 └── README.md

📸 Screenshots (Placeholders)

Add screenshots in your GitHub later.

Home Page

Filters Panel

Product Cards

Floating Cart

Mobile View

🎓 Learning Outcomes

By completing this project, you will gain experience in:

✔ JavaScript DOM manipulation
✔ Event-driven programming
✔ Client-side product filtering logic
✔ Responsive web design
✔ UI/UX design
✔ Bootstrap 5 layout mastery
✔ Working with arrays & data structures

🔮 Future Enhancements

Backend integration (Node.js / Firebase)

User login & authentication

Database-driven product list

Pagination

Dark/Light mode sync

Add to cart persistence (LocalStorage)

API-based filters#
