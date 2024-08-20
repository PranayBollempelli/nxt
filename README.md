# Nxt Trendz - Cart Features

This project is a part of the **Nxt Trendz** application, focusing on implementing key cart functionalities using React. The app simulates an e-commerce platform, where users can add, update, and manage items in their cart.

## Features

1. **Authentication**
   - **Login Required**: Access to the cart is restricted to authenticated users. If an unauthenticated user attempts to view the cart, they will be redirected to the Login page.

2. **Cart Management**
   - **Add to Cart**: Users can add products to the cart. If the same product is added multiple times, its quantity will be updated rather than adding it as a new item.
   - **Cart Summary**: The cart displays the total number of items and the total cost of the products added.

3. **Quantity Adjustment**
   - **Increment/Decrement Quantity**: Users can increase or decrease the quantity of products in their cart.
     - If the quantity is increased, the cart total is updated accordingly.
     - If the quantity is decreased and reaches one, clicking the decrement button will remove the item from the cart.

4. **Remove Items**
   - **Remove Item**: Users can remove individual items from the cart.
   - **Remove All**: Users have the option to clear the entire cart with a single click, leading to an empty cart view.

## Cart Context API

The cart features are managed using a custom Cart Context, providing the following methods:

- `cartList`: Stores all items in the cart.
- `removeAllCartItems`: Clears all items from the cart.
- `addCartItem`: Adds a new item to the cart or updates the quantity if it already exists.
- `removeCartItem`: Removes a specific item from the cart.
- `incrementCartItemQuantity`: Increases the quantity of a cart item.
- `decrementCartItemQuantity`: Decreases the quantity of a cart item.

## Component Structure

The app is structured into the following components:

- **Cart**: The main cart component that displays all items and the cart summary.
- **CartItem**: Represents an individual item in the cart, allowing quantity adjustment or removal.
- **CartSummary**: Displays the total number of items and the total cost.

## Setup Instructions

To run the project locally:

1. Clone the repository.
2. Install the dependencies using `npm install`.
3. Start the application using `npm start`.

## Design

The app is designed to be responsive, with different layouts for small, medium, and large screen sizes. Design references can be found in the provided design files.

## Important Notes

- The project uses icons from `react-icons` for plus, minus, and remove actions.
- Test accounts for different user roles are provided:
  - **Prime User**: `username: rahul`, `password: rahul@2021`
  - **Non-Prime User**: `username: raja`, `password: raja@2021`

## Resources

- **Colors**: The project uses a set of predefined colors, including `#0b69ff`, `#171f46`, `#616e7c`, and `#ffffff`.
- **Font**: The project uses the Roboto font.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
