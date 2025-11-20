# 🛍️ Lumina | Modern E-Commerce UI

Lumina is a sleek, modern, single-page E-Commerce application designed to showcase a clean user interface and vanilla JavaScript application logic.

This project uses no frameworks, demonstrating how to build a dynamic shopping experience, including product filtering, a functional cart, and a multi-step checkout process, using only native browser capabilities.

## ✨ Features

* **Single-Page Application (SPA) Logic:** Manages three distinct views (`Shop`, `Checkout`, `Success`) using pure JavaScript state management.
* **Dynamic Product Grid:** Products are rendered from a JavaScript array (`PRODUCTS`) and include interactive elements.
* **Filtering & Search:** Users can filter products by category and search by name in real-time.
* **Full Shopping Cart:** Add, remove, and update item quantities in a responsive side-drawer.
* **Checkout Flow:** Transitions from the cart to a simulated checkout and final success page.
* **Responsive Design:** Styled using **Tailwind CSS** for a great experience on desktop and mobile.
* **Modern Styling:** Utilizes Tailwind CSS utility classes, custom CSS for animations (`fade-in`, `slide-in-right`), and **Lucide Icons** for a clean look.

## 🛠️ Tech Stack

* **HTML5:** Structure of the application.
* **Tailwind CSS:** Utility-first CSS framework for rapid styling. (Included via CDN)
* **Vanilla JavaScript (ES6+):** All application logic, state management, DOM manipulation, and event handling.
* **Lucide Icons:** Open-source icon set for visual elements. (Included via CDN)

## 🚀 Getting Started

Lumina is a purely client-side application and does not require a build process or server.

### Prerequisites

You only need a modern web browser.

### Installation

1.  **Clone the repository (or download the `index.html` file):**
    ```bash
    git clone [https://github.com/your-username/Lumina-Ecommerce-UI.git](https://github.com/your-username/Lumina-Ecommerce-UI.git)
    cd Lumina-Ecommerce-UI
    ```
2.  **Open the file:**
    Simply double-click the `index.html` file in your file explorer, and it will open in your default web browser.

## 📂 Project Structure

The entire application is contained within a single `index.html` file:
### Key JavaScript Areas (`<script>` block)

| Section | Purpose |
| :--- | :--- |
| **`PRODUCTS` & `CATEGORIES`** | The raw data source for the E-Commerce store. |
| **`app.state`** | The central state object (cart, view, filters) for the SPA logic. |
| **`app.setView(viewName)`** | Function responsible for hiding/showing the main views (`shop`, `checkout`, `success`). |
| **`app.renderProducts()`** | Manages filtering (`searchQuery` & `selectedCategory`) and renders the product cards to the DOM. |
| **`app.updateCartUI()`** | Calculates totals and renders the cart items in the side drawer. |
| **`app.handleCheckoutSubmit()`**| Simulates a payment delay and resets the cart before navigating to the success view. |

## 📐 Styling & Design

The design philosophy focuses on minimalism, good typography, and clear calls-to-action.

* **Color Palette:** Primarily uses `slate` for background/text and `blue` for primary accents.
* **Custom Utilities:** Custom CSS is included in the `<style>` block to manage scrollbar hiding (`no-scrollbar`) and create smooth transitions between views (`fade-in`, `slide-in-right`).
* **Sticky Elements:** The main navigation bar and the product filter bar are sticky for easy access while scrolling.

## 🤝 Contribution

Feel free to fork this project, experiment with new features, or suggest improvements to the UI/UX or JavaScript logic!

## 📄 License

This project is open-source.