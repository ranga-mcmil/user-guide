# User Guide: New Inventory Management Features

## Welcome to the New Inventory System! 🎉

This guide will help you learn how to use the new inventory management features that have been added to Roofstar. These features help you better track your products, manage batches, and handle customer orders more efficiently.

## What's New?

### 📊 Product Formulas
**What it is**: Mathematical formulas that help calculate product specifications automatically.

**Why it matters**: Instead of manually calculating dimensions for each product, you can create a formula once and reuse it for similar products.

**How to use**:
1. Go to **Products** → **Manage Attributes** → **Product Formulas**
2. Click **"Create Formula"**
3. Give your formula a name (like "Standard IBR Formula")
4. Enter the formula value (like 3.6 for length calculations)
5. Click **"Create Formula"**

**Example**: If you have many IBR sheets that all use the same length calculation, create one formula and use it for all similar products.

### 📦 Batch Items
**What it is**: Individual items within a batch that you can track separately.

**Why it matters**: You can now track exactly which specific items from which batch are being sold to customers.

**How to use**:
1. Go to **Batch Items** in the main menu
2. Click **"Create Batch Item"**
3. Select the batch this item belongs to
4. Choose the item type:
   - **Length/Width**: For sheets with specific dimensions
   - **Weight**: For items sold by weight
   - **Quantity**: For countable items (like screws)
   - **Unknown**: For items without specific measurements
5. Fill in the specifications (dimensions, weight, quantity)
6. Add any notes
7. Click **"Create Batch Item"**

**Example**: If you have a batch of 100 IBR sheets, you can create 100 batch items and track each one individually.

### 🏷️ Codes
**What it is**: Product codes that help identify and organize your inventory.

**Why it matters**: Consistent coding makes it easier to find products and avoid confusion.

**How to use**:
1. Go to **Codes** in the main menu
2. Click **"Create Code"**
3. Enter a code (like "IBR-047-CH" for IBR 0.47mm Charcoal)
4. Add a description
5. Click **"Create Code"**

**Example**: Use codes like "IBR-047-CH" for IBR sheets, "ACC-RC-GL" for accessories, etc.

### 🔗 Allocations
**What it is**: The process of assigning specific batch items to customer orders.

**Why it matters**: You can now track exactly which items from which batch are being sold, making inventory management more precise.

**How to use**:
1. When processing an order, go to **Allocations** → **Order Allocations**
2. Select the order you want to allocate items for
3. For each order item, choose which batch items to allocate
4. Enter the quantity to allocate
5. Click **"Allocate"**

**Example**: When a customer orders 10 IBR sheets, you can allocate 10 specific sheets from a particular batch.



## Step-by-Step Workflows

### Creating a New Product with Formula
1. Go to **Products** → **Create Product**
2. Fill in basic information (name, price, etc.)
3. Select a formula from the dropdown
4. Choose the product type
5. Set referable status and percentage
6. Enter the product code as text
7. Click **"Create Product"**

### Processing an Order with Allocations
1. Go to **Orders** page
2. Find the order you want to allocate items for
3. Either:
   - Click the **"Manage Allocation"** button in the orders table, OR
   - Click on the order row to view details, then click **"Manage Allocation"** button
4. For each order item:
   - Select the order item
   - Choose available batch items
   - Enter quantity to allocate
   - Click **"Allocate"**
5. Review the allocations
6. Complete the order

### Managing Batch Items
1. Go to **Batch Items**
2. Use the search bar to find specific items
3. Filter by batch number or type
4. Click on any item to view details
5. Edit or delete as needed


