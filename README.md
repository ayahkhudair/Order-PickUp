# OrderPick
OrderPick is a Java Swing mobile-style app for food ordering. It features MySQL integration, role-based access for Admins and Customers, and a secure payment gateway. Users can register, browse a categorized menu, and manage a cart. The system generates digital receipts with pickup codes and allows admins to track live orders and staff data.

<!DOCTYPE html>
<html>
<body>

  <h1>🍔 OrderPick</h1>
  <p>
    <strong>OrderPick</strong> is a Java Swing-based desktop application designed with a <strong>mobile-first aesthetic</strong>. It streamlines the food ordering process, allowing users to browse menus, manage a cart, and securely process payments, while providing administrators with tools to manage live orders and staff.
  </p>

  <h2>🚀 Key Features</h2>
  <ul>
    <li><strong>User Roles:</strong> Separate interfaces for Customers (ordering) and Admins (management).</li>
    <li><strong>Secure Auth:</strong> Custom registration and login system with MySQL integration and <code>LoginFailedException</code> handling.</li>
    <li><strong>Digital Menu:</strong> Dynamic menu loading with categorized items (Burgers, Sides, Drinks).</li>
    <li><strong>Checkout Flow:</strong> Integrated <code>CreditCardPaymentWindow</code> with real-time card validation (Regex &amp; Expiry checks).</li>
    <li><strong>Digital Receipts:</strong> Generates unique Order IDs and Pickup Codes, with an option to save receipts as <code>.txt</code> files.</li>
    <li><strong>Admin Panel:</strong> Real-time oversight of the <code>order</code>, <code>menuitem</code>, and <code>admin</code> database tables.</li>
  </ul>

  <h2>🛠️ Tech Stack</h2>
  <ul>
    <li><strong>Language:</strong> Java</li>
    <li><strong>GUI Framework:</strong> Swing / AWT</li>
    <li><strong>Database:</strong> MySQL</li>
    <li><strong>Architecture:</strong> Object-Oriented (Inheritance, Custom Exceptions, Encapsulation)</li>
  </ul>

  <h2>📸 UI Specifications</h2>
  <ul>
    <li><strong>Resolution:</strong> 360x640 (Mobile Portrait Mode).</li>
    <li><strong>Theme:</strong> Modern "Food-Tech" palette (Red #C81E1E and Beige #F5EBDC).</li>
  </ul>

  <h2>📦 Project Structure</h2>
  <pre>
  ├── src/
  │   ├── AdminDashboard.java      # Admin management interface
  │   ├── CustomerDashboard.java   # Ordering & Cart system
  │   ├── LoginWindow.java         # Authentication entry point
  │   ├── CreditCardPaymentWindow.java # Payment validation logic
  │   ├── bill.java                # Receipt generation and File I/O
  │   └── AppColors.java           # Centralized UI styling
  </pre>

  <h2>⚙️ Setup</h2>
  <ol>
    <li>Clone the repository.</li>
    <li>Ensure you have a MySQL server running with a database named <code>project</code>.</li>
    <li>Update the DB credentials in <code>RegisterWindow.java</code> and <code>LoginWindow.java</code>.</li>
    <li>Run <code>OrderPickupApp.java</code> to start the application.</li>
  </ol>

</body>
</html>
