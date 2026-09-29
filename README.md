# Nova Market

Nova Market is a responsive ecommerce storefront designed for customers to browse products, add items to a shopping cart, and complete a checkout flow using M-PESA. The website also provides customer support, complaints handling, and a seller area for adding products.

## Main Features

### 1. Product Marketplace
The Shop section displays products in a responsive product grid. Customers can:

- Browse available products.
- Filter products by category.
- Search for products by name.
- View product names and prices in Kenyan Shillings (KES).
- Add products to the shopping cart.
- Add new products through the Sell section.

The current catalog includes products such as:

- Aero Pro Wireless Headphones
- Orbit S2 Smartwatch
- Cloud Runner 02
- Kivu Leather Crossbody
- Sienna Ceramic Coffee Set
- Halo Ambient Table Lamp
- Hydra Steel Bottle 750ml
- Atlas Weekender

## 2. Shopping Cart

Customers can add products to the cart and manage their order before checkout.

Cart functionality includes:

- Increasing or decreasing quantities.
- Removing products.
- Restoring a recently removed product.
- Calculating the subtotal.
- Calculating delivery charges.
- Calculating the total amount.
- Displaying the number of items in the cart.

Delivery is configured so that orders of KES 3,000 or more receive free delivery. Orders below that amount use the configured KES 250 delivery charge.

## 3. M-PESA Checkout

The checkout interface is designed around M-PESA payments.

Customers enter:

- Full name
- M-PESA/Safaricom phone number
- Delivery address

The interface validates the required information and provides an M-PESA payment flow.

**Important:** In the current standalone preview, the payment experience is a demonstration interface. A production website must connect the checkout to a secure backend and a real M-PESA Daraja/API integration. Payment credentials and API secrets should never be placed in the frontend HTML or JavaScript.

## 4. Vertical Sidebar

Nova Market uses a vertical navigation sidebar instead of placing all of the main sections in the top navigation.

The sidebar contains:

- **Shop** — browse products.
- **Categories** — browse products by type.
- **Our Story** — information about Nova Market.
- **Reviews** — customer review content.
- **Support** — help and customer assistance.
- **Sell** — area for adding/listing a product.

The sidebar can be expanded and retracted to give the main shopping area more room.

On smaller screens, the layout adapts to the available screen width.

## 5. Support

The Support area provides customer assistance features including:

- Frequently asked questions.
- Help Centre information.
- Order history information.
- Payment help.
- Contact/support guidance.

## 6. Complaints

Customers can submit a complaint when they experience a problem with an order.

Complaint functionality includes:

- Selecting an order.
- Selecting the type of problem.
- Writing a description of the issue.
- Generating a complaint reference.
- Viewing previously submitted complaints.
- Showing the complaint status.

Example complaint categories include:

- Item or service not delivered.
- Wrong or damaged item.
- Poor service quality.
- Overcharged/payment issue.
- Other.

## 7. Sell / Add Product

The Sell section allows a seller to add a product to the storefront.

Product information can include:

- Product name.
- Category.
- Price in KES.
- Product photo.
- Other product information supported by the interface.

Uploaded product images can be previewed before the product is added.

For a production marketplace, product creation should be connected to a secure database and authenticated seller account.

## 8. Responsive Design

The website is designed to work across:

- Desktop computers.
- Laptops.
- Tablets.
- Mobile phones.

The product grid automatically adjusts to the available screen width, while the sidebar adapts for smaller displays.

## 9. Accessibility

The interface includes accessibility-oriented features such as:

- Semantic navigation and content structure.
- ARIA labels where appropriate.
- Keyboard interaction for dialogs and menus.
- Focus handling for modal interfaces.
- Reduced-motion support.
- Screen-reader announcements for important actions.

## 10. Browser Storage

The current standalone version uses browser `localStorage` for several pieces of demo state, including:

- Shopping cart.
- Orders.
- Complaints.
- Other temporary customer interaction data.

This means the information is stored locally in the browser rather than in a shared online database.

Clearing browser storage or changing browsers/devices can remove or prevent access to this locally stored data.

## 11. Production Requirements

The current HTML file is a frontend preview/prototype. To turn Nova Market into a production ecommerce platform, the following should be connected to a secure backend:

- User authentication.
- Seller authentication and permissions.
- Product database.
- Product inventory/stock management.
- Customer accounts.
- Orders and order items.
- Secure M-PESA payment processing.
- Payment callbacks/webhooks.
- Complaint management.
- Image storage.
- Admin controls.
- Server-side validation.
- Database backups.
- Security and access controls.

Sensitive credentials, payment keys, database credentials, and server secrets must remain on the server.

## 12. Running the Website

The current version is a standalone HTML website.

### Quick preview

1. Download the HTML file.
2. Open the HTML file in a modern web browser.
3. Browse the Shop section.
4. Use the sidebar to navigate around the website.
5. Add products to the cart.
6. Test the checkout interface.

For a production deployment, the site should be served through a web server/hosting platform and connected to the required backend services.

## Project Purpose

Nova Market is intended to provide a modern, simple ecommerce experience focused on product discovery, shopping, M-PESA-oriented checkout, customer support, complaints, and seller product listing.

The current standalone version is suitable for demonstrating the user interface and frontend interactions. Production payment, authentication, database, inventory, and administrative functionality require secure backend implementation.
