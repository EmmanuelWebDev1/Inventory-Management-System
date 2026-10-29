STOCKPILOT INVENTORY MANAGEMENT SYSTEM
=======================================

Features
- Dashboard: product count, units, stock valuation and low-stock alerts
- Product management: add, edit, search and archive products
- Stock-in and stock-out transactions with reference and notes
- Automatic quantity updates; stock-outs cannot exceed available stock
- Transaction history and stock valuation reports
- Print / Save PDF report
- Responsive interface for desktop and mobile
- MySQL database with PDO prepared statements and CSRF checks on forms

Tech stack: PHP 8+, MySQL/MariaDB, HTML, CSS, vanilla JavaScript.

Install with XAMPP on Windows
1. Start Apache and MySQL in the XAMPP Control Panel.
2. Extract this folder into C:\xampp\htdocs\ so the path is
   C:\xampp\htdocs\inventory-management-system\
3. Visit http://localhost/phpmyadmin
4. Use Import and select database/inventory.sql from this project.
   It creates inventory_management and adds sample products.
5. Check config/database.php. Defaults: host localhost, database
   inventory_management, username root, blank password. Update if needed.
6. Open http://localhost/inventory-management-system/

How to use
- Products: create products with unique SKUs, costs, quantities and reorder levels.
- Stock transactions: select Stock in to receive items or Stock out to issue them.
- Reports: review current valuation and use Print / Save PDF.

Important
- This is a portfolio/demo project and does not include login/authentication.
  Add authentication and authorization before deploying publicly.
- Sample products are inserted by the SQL file; edit or archive them as needed.
- Inventory value = current quantity × unit cost.
- Archived products are hidden from the active catalog; transaction history remains.
