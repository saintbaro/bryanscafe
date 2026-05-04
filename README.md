# Bryan's Café ☕

## Overview
A responsive, multi-page website built for the Diploma unit **ICTWEB441 & ICTWEB518**. This project demonstrates the implementation of client-side scripting (JavaScript) and the utilization of Extensible Markup Language (XML) to dynamically load, parse, and display structured data in a modern web environment.

## 🌟 Features

- **Dynamic Data Rendering (XML to HTML)**: 
  - The Menu (`menu.html`) fetches structured data from `xml/menu.xml` and parses it via `DOMParser` to automatically generate categorized items.
  - The Branches list (`contact.html`) fetches location data from `branches.xml` to populate the map links and addresses.
- **Responsive Web Design**: 
  - Built from the ground up to support desktops, tablets, and mobile devices using CSS Flexbox, Grid, and targeted media queries.
  - Features a custom interactive hamburger menu for smaller viewports.
- **Bootstrap 5 Integration**: Employs Bootstrap's Accordion and Card systems on the Menu page for an organized, space-saving UI, controlled entirely by custom JavaScript logic.
- **Form Handling**: A client-side contact form that requires standard inputs and utilizes JavaScript to simulate a successful submission and form reset.
- **Document Type Definitions (DTD)**: Ensures strict structural validity of the XML data using custom `.dtd` schemas.

## 📂 Project Structure

```text
📁 Bryan's Café/
├── 📄 index.html        # Landing page with About and History sections
├── 📄 menu.html         # Dynamically renders XML menu items into an Accordion
├── 📄 contact.html      # Enquiry form and dynamically rendered branch locations
├── 📄 privacy.html      # Privacy policy
├── 📄 style.css         # Core styles, media queries, and layout formatting
├── 📄 script.js         # Global interactions (e.g., mobile hamburger menu toggle)
├── 📄 branches.xml      # XML database containing branch locations and details
├── 📄 branches.dtd      # Document Type Definition for branches
└── 📁 xml/              
    ├── 📄 menu.xml      # XML database containing categorized menu items
    └── 📄 menu.dtd      # Document Type Definition for the menu
```

## 🚀 How to Run Locally

Because this project utilizes the JavaScript `fetch` API to load local XML files, opening the HTML files directly from your hard drive (`file:///...`) will trigger browser CORS security restrictions. 

To view the dynamic content correctly:
1. Open the project folder in a code editor like **Visual Studio Code**.
2. Install a local server extension (such as **Live Server**).
3. Right-click `index.html` and select **"Open with Live Server"**.
4. The site will launch in your browser (typically at `http://127.0.0.1:5500`) and the XML data will load flawlessly!

## 🎓 Unit Requirements Met
- **ICTWEB441**: Produced basic client-side scripts to manipulate the Document Object Model (DOM) and add interactivity.
- **ICTWEB518**: Built and integrated documents using Extensible Markup Language (XML) and validated them against DTD rules.