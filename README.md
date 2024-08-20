# Nxt Trendz - E-commerce Application

This project is a comprehensive **E-commerce Application** built using React on the frontend and a Node.js/Express backend. It focuses on key functionalities like authentication, product management, and a dynamic shopping cart system, providing a full-stack solution for an online retail platform.

## Overview

The **Nxt Trendz** application simulates an end-to-end e-commerce experience where users can browse products, manage their shopping carts, and proceed through checkout. This project particularly emphasizes the cart management features, ensuring a seamless and responsive user experience.

## Features

### 1. Full-Stack Implementation
- **Frontend**: Built with React, the frontend is designed to be responsive and interactive, providing a smooth user interface for managing product listings and the shopping cart.
- **Backend**: The backend is powered by Node.js and Express, handling user authentication, product data management, and API integration for cart functionalities.

### 2. Authentication
- **User Login/Signup**: The application supports user authentication with login and signup features. Users must be logged in to add items to the cart and proceed to checkout.
- **Access Control**: Unauthorized users are redirected to the login page if they attempt to access protected routes like the cart or checkout pages.

### 3. Product Management
- **Product Listing**: The application dynamically loads product data, displaying it in a responsive grid layout. Users can view product details and add items to their cart.
- **Search and Filter**: Users can search for products by name and filter results based on categories or other criteria.

### 4. Cart Management
- **Add to Cart**: Users can add products to their cart. If the same product is added multiple times, its quantity is updated instead of creating duplicate entries.
- **Cart Summary**: The cart displays the total number of items and the cumulative cost of products, updating in real-time as users modify their cart.
- **Quantity Adjustment**: Users can increment or decrement product quantities directly in the cart. If the quantity of an item is reduced to one and the decrement button is clicked again, the item is removed from the cart.
- **Remove Items**: Individual items or all items can be removed from the cart with ease.
- **Persistent Cart**: The cart state is preserved across sessions, allowing users to resume shopping where they left off.

### 5. Checkout Process
- **Order Summary**: Before completing a purchase, users can review their order, including item quantities and total cost.

## Cart Context API

The cart functionalities are managed using a custom Cart Context in React, which provides the following methods:

- `cartList`: Manages the list of items currently in the cart.
- `addCartItem`: Adds a product to the cart or updates its quantity if it already exists.
- `removeCartItem`: Removes a specific product from the cart.
- `incrementCartItemQuantity`: Increases the quantity of a product in the cart.
- `decrementCartItemQuantity`: Decreases the quantity of a product in the cart, with the option to remove the item if the quantity reaches zero.
- `removeAllCartItems`: Clears all items from the cart.

## Component Structure

The application is divided into several key components:

- **ProductList**: Displays available products in a grid format.
- **ProductDetails**: Shows detailed information about a selected product.
- **Cart**: The main component that handles cart interactions and displays the cart summary.
- **CartItem**: Represents individual products in the cart, allowing users to adjust quantities or remove items.
- **CartSummary**: Provides a summary of the cart, including the total number of items and total cost.

## Setup Instructions

To run the project locally:

1. Clone the repository.
2. Install the dependencies for both frontend and backend using `npm install` in their respective directories.
3. Start the backend server with `npm run start` in the backend directory.
4. Start the frontend application with `npm start` in the frontend directory.
5. The application will be available at `http://localhost:3000`.

## Design

- **Responsive Design**: The application is fully responsive, offering an optimal viewing experience across a wide range of devices (from mobile phones to desktop computers).
- **UI/UX**: The design emphasizes user experience, ensuring easy navigation and a visually appealing interface.

## Important Notes

- The project uses icons from `react-icons` for user interface elements like increment, decrement, and remove actions.
- Test accounts are provided for different user roles:
  - **Prime User**: `username: rahul`, `password: rahul@2021`
  - **Non-Prime User**: `username: raja`, `password: raja@2021`
- The backend includes sample data for products and users to facilitate testing and demonstration.

## Resources

- **Colors**: The application uses a consistent color palette, including `#0b69ff`, `#171f46`, `#616e7c`, and `#ffffff`.
- **Font**: The Roboto font is used throughout the application for a clean and modern look.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
