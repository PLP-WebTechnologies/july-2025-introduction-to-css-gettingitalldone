# 🎨 Assignment: CSS Basics & The Box Model

## Overview

This assignment introduces you to the foundational principles of CSS—how to style web content, apply essential styling properties, and understand the powerful concept of the CSS Box Model. You’ll practice writing clean, organized CSS that brings structure and visual appeal to an HTML page.

## Objective

Your goal is to create a visually styled web page using only CSS. You will apply basic styling rules to text, backgrounds, and layout elements, and demonstrate an understanding of how the CSS Box Model affects spacing and sizing on the page.

## What You'll Practice

* Connecting CSS to your HTML (external stylesheet)
* Using basic CSS properties such as `color`, `font-size`, `margin`, `padding`, `border`, and `background`
* Structuring your layout with awareness of how the Box Model influences spacing and dimensions
* Writing clean and maintainable CSS selectors and rules

## Instructions

Start with a basic HTML structure and create a separate CSS file named `styles.css`. Link it to your HTML file. Apply various styles to headings, paragraphs, and container sections.

Use the Box Model deliberately—experiment with margin, padding, and borders to see how they affect the layout. Apply background colors to visualize box boundaries. You may also style buttons, navigation, and card-like sections to demonstrate your grasp of spacing and alignment.

No JavaScript or external CSS libraries (like Bootstrap) should be used.

## Deliverables

Submit the following files:

* `index.html`: A basic HTML page with structured content.
* `styles.css`: Your external stylesheet containing all your CSS rules.

Both files should work together to showcase:

* Proper use of selectors and basic styling properties
* Clear implementation of the CSS Box Model
* Consistent spacing, sizing, and layout styling

## Tips

* Correct linkage of HTML and CSS files
* Use of appropriate CSS selectors and properties
* Demonstration of the Box Model through visual layout (clear use of margin, padding, and borders)
* Readability and organization of CSS code (indentation, comments, spacing)
* Overall appearance and clarity of styled content
Understood — we'll keep everything **pure HTML and CSS**, with **no JavaScript** or **external libraries** like Bootstrap.

Here’s a final, clean version of the project that meets all your requirements:

* Uses the **CSS Box Model** with margin, padding, border, background.
* Styles **headings, paragraphs, buttons, nav, and card sections**.
* Avoids any **JavaScript** or **external CSS libraries**.

---

##  `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Pure CSS Box Model Demo</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>

  <!-- Navigation Bar -->
  <nav class="navbar">
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <!-- Main Container -->
  <div class="container">
    <h1>Welcome to the Box Model Demo</h1>
    <p>This container demonstrates margin, padding, and borders using plain CSS.</p>
    <button class="btn">Explore More</button>
  </div>

  <!-- Card Section -->
  <section class="cards">
    <div class="card">
      <h2>Card One</h2>
      <p>This card has padding, margin, border, and background color for visualization.</p>
    </div>
    <div class="card">
      <h2>Card Two</h2>
      <p>Spacing between cards is managed using margin and flexbox gap.</p>
    </div>
    <div class="card">
      <h2>Card Three</h2>
      <p>Using only HTML and CSS, no JavaScript or external frameworks involved.</p>
    </div>
  </section>

</body>
</html>
```

---

##  `styles.css`

```css
/* Reset default styles */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

/* Body styling */
body {
  font-family: sans-serif;
  background-color: #f9f9f9;
  line-height: 1.6;
}

/* NAVIGATION BAR */
.navbar {
  background-color: #222;
  padding: 15px 0;
}

.navbar ul {
  display: flex;
  justify-content: center;
  list-style: none;
  gap: 40px;
}

.navbar a {
  color: white;
  text-decoration: none;
  padding: 8px 16px;
  border: 2px solid transparent;
}

.navbar a:hover {
  border-color: white;
  background-color: #444;
}

/* MAIN CONTAINER */
.container {
  background-color: #ffffff;
  border: 2px solid #cccccc;
  padding: 20px;
  margin: 30px auto;
  width: 85%;
  max-width: 800px;
  border-radius: 8px;
  box-shadow: 0 0 10px rgba(0,0,0,0.05);
}

/* HEADINGS AND PARAGRAPH */
h1 {
  color: #2c3e50;
  margin-bottom: 15px;
}

p {
  color: #555555;
  margin-bottom: 20px;
}

/* BUTTON STYLES */
.btn {
  background-color: #3498db;
  color: white;
  padding: 12px 20px;
  border: 2px solid #2980b9;
  border-radius: 5px;
  cursor: pointer;
}

.btn:hover {
  background-color: #2980b9;
}

/* CARD SECTION */
.cards {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
  margin: 40px auto;
  width: 90%;
}

.card {
  background-color: #eef6ff;
  border: 2px dashed #3498db;
  padding: 20px;
  width: 280px;
  border-radius: 10px;
  box-shadow: 2px 2px 6px rgba(0,0,0,0.05);
}

.card h2 {
  color: #2980b9;
  margin-bottom: 10px;
}

.card p {
  color: #444;
}
```

---

##  Box Model Visualized

* **`padding:`** Adds internal space within elements (inside border).
* **`margin:`** Creates space between elements.
* **`border:`** Defines the edge of the box.
* **`background-color:`** Highlights each element's box boundary.

---

##  Folder Structure

```
box-model-demo/
├── index.html
└── styles.css
```

---


