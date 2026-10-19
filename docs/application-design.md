# Database and Application Design

## Source and verification

This case study is based on the student's **Database Application Assignment 1 – Online Shopping System**, completed at Webster University in Tashkent on **17 September 2026**.

The evidence documents a working Oracle APEX application. This repository is **not** an Oracle APEX export and cannot recreate the original application by itself.

## Data structures documented

| Table | Attributes shown in the report | Purpose |
| --- | --- | --- |
| `SHOP_CUSTOMERS` | `CUSTOMER_ID`, `FULL_NAME`, `EMAIL`, `PHONE`, `CITY`, `REGISTERED_ON` | Customer management and forms |
| `SHOP_PRODUCTS` | `PRODUCT_ID`, `PRODUCT_NAME`, `CATEGORY`, `PRICE`, `STOCK_QUANTITY`, `BRAND` | Catalog and editable inventory |
| `SHOP_ORDERS` | `ORDER_ID`, customer ID, order date, status, payment method, shipping address | Orders and status reporting |
| `SHOP_ORDER_ITEMS` | `ORDER_ITEM_ID`, order ID, product ID, quantity, unit price, optional note | Order line details |

The report shows primary-key columns. Without an Oracle schema or export, this documentation does **not** claim that all foreign-key relationships have been independently verified.

## Navigation and pages

The main sections are **Customers, Products, Orders, and Order Items**, each with two submenus and third-level links:

- Customers → Customer Records / Customer Orders
- Products → Product Catalog / Stock Management
- Orders → Order Records / Order Analytics
- Order Items → Item Records / Related Products

Home, Charts, and Inventory Grid are additional application destinations. The report documents **23 navigation entries** in total.

## Functionality demonstrated in coursework

1. Browse customer, product, order, and order-item reports.
2. Open the **Create Customer** form and add a test record.
3. Observe the customers list grow from 10 to 11 entries.
4. Edit an existing customer's city and confirm that the record is updated rather than duplicated.
5. Inspect the **Inventory Grid** with editing and saving controls.
6. Review a bar chart showing **Delivered: 3**, **Shipped: 2**, **Processing: 2**, **Pending: 2**, and **Cancelled: 1** orders.

## Public portfolio scope

This repository shows an academic case study with sanitized screenshots. It does **not** include running Oracle APEX source code, a database dump, private workspace URLs, real customer records, or credentials.

A future enhancement would be a reviewed and sanitized Oracle APEX application export, plus documentation describing how to import it into a test workspace.

## Relevant skills

Oracle APEX, Oracle Database fundamentals, relational database modeling, CRUD forms, interactive reports, low-code application development, data visualization, and navigation design.
