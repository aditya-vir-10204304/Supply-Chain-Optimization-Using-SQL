1. Project Description

     This project demonstrates the use of SQL to analyze and optimize supply chain operations. By simulting real-world dat for suppliers, products, inventory, and orders, it highlights key      insights such as uspplier performance, inventory management, and order tracking. The project showcases advanced SQL techniques, including joins grouping, and aggregate functions, 
     to solve supply chain-related business challenges effectively.

2. Database Schema

a. Suppliers

| **Column Name**  | **Data Type** | **Description**            |
|------------------|---------------|----------------------------|
| SupplierID       | INTEGER       | Primary key, unique ID for each supplier. |
| Name             | TEXT          | Name of the supplier.      |
| Region           | TEXT          | Geographic region of the supplier. |
| ContactNumber    | TEXT          | Phone number of the supplier. |
| Rating           | REAL          | Rating score for the supplier. |

b. Products

| **Column Name**  | **Data Type** | **Description**            |
|------------------|---------------|----------------------------|
| ProductID        | INTEGER       | Primary key, unique ID for each product. |
| Name             | TEXT          | Name of the product.       |
| Category         | TEXT          | Category of the product.   |
| UnitCost         | REAL          | Cost per unit of the product. |

c. Inventory

| **Column Name**     | **Data Type** | **Description**                    |
|---------------------|---------------|------------------------------------|
| ProductID           | INTEGER       | Foreign key, references Products. |
| StockLevel          | INTEGER       | Current stock level for the product. |
| ReorderLevel        | INTEGER       | Threshold stock level to trigger reordering. |
| WarehouseLocation   | TEXT          | Location of the product in the warehouse. |

d. Orders

| **Column Name**  | **Data Type** | **Description**                    |
|------------------|---------------|------------------------------------|
| OrderID          | INTEGER       | Primary key, unique ID for each order. |
| SupplierID       | INTEGER       | Foreign key, references Suppliers. |
| ProductID        | INTEGER       | Foreign key, references Products. |
| OrderDate        | TEXT          | Date the order was placed.        |
| DeliveryDate     | TEXT          | Date the order was delivered.     |
| Quantity         | INTEGER       | Quantity of products ordered.     |
| TotalCost        | REAL          | Total cost of the order.          |

3. Relationships

![ERD Diagram]("C:\Users\Aditya Vir\Downloads\SCOERD.png")
