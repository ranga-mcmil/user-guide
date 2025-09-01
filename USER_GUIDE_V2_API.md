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

## Updated Product Management

### New Product Fields
When creating or editing products, you'll now see these new fields:

- **Formula**: Choose a formula for automatic calculations
- **Type**: Select how the product is measured (Length/Width, Weight, Quantity, Unknown)
- **Referable**: Check if this product is eligible for referral commissions
- **Referrable Percentage**: Set the commission percentage for referrals

### Product Table Changes
The products table now shows:
- Formula name
- Product type
- Referable status (with a badge)

## Navigation Changes

### New Menu Items
You'll see these new options in the main menu:
- **Codes** (for Admin and Manager roles)
- **Batch Items** (for Admin and Manager roles)
- **Product Formulas** (under Products → Manage Attributes)

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
1. Create the order as usual
2. Go to **Allocations** → **Order Allocations**
3. Find your order in the list
4. For each item in the order:
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

## Tips and Best Practices

### For Better Organization
- **Use consistent codes**: Create a naming system for your codes (like "IBR-047-CH" for IBR 0.47mm Charcoal)
- **Create reusable formulas**: If you have many similar products, create one formula and reuse it
- **Track everything**: Allocate batch items to orders whenever possible for better inventory tracking

### For Different User Roles
- **Admin**: You have access to all features
- **Manager**: You have access to most features, with some limitations based on your branch
- **Sales Rep**: You have limited access, mainly for allocations and basic features

## Common Tasks

### Finding a Product
1. Go to **Products**
2. Use the search bar to find by name or code
3. Click on the product row to view details

### Checking Allocations
1. Go to **Allocations** → **Order Allocations**
2. Find the order you're interested in
3. View the allocation details for each item

### Exporting Data
- Most pages have an **"Export"** button
- Click to download data as CSV file
- Useful for reports and analysis

## Troubleshooting

### Common Issues

**"Formula not found"**
- Make sure you've created the formula first
- Go to Products → Manage Attributes → Product Formulas

**"Batch item not available"**
- Check if the batch item has enough quantity
- The system won't let you allocate more than what's available

**"Code already exists"**
- Use a unique code for each product
- Check existing codes in the Codes section

### Getting Help
- Check the browser console for error messages
- Contact your system administrator for technical issues
- Refer to this guide for step-by-step instructions

## What's Different from Before?

### Major Changes
- **Product codes**: Now text instead of numbers
- **Stock tracking**: Replaced with a more detailed allocation system
- **New fields**: Products now have formulas, types, and referral settings
- **Better organization**: More structured way to manage inventory

### What Stays the Same
- Basic product management workflow
- Order creation process
- User interface design and layout
- Most existing features and functionality

## Quick Reference

### Common Actions
- **Create new item**: Look for "Create" buttons on list pages
- **Edit item**: Click on any row in a table
- **Delete item**: Use the delete button on detail pages
- **Export data**: Use the export button on list pages

### Important URLs
- `/codes` - Manage product codes
- `/product-formulas` - Manage formulas
- `/batch-items` - Manage batch items
- `/allocations/order/[orderNumber]` - Allocate items to orders

### Keyboard Shortcuts
- Use **Tab** to navigate between fields
- Use **Enter** to submit forms
- Use **Escape** to cancel actions

---

## Need Help?

If you have questions about using these new features:
1. Check this guide first
2. Ask your team lead or manager
3. Contact the IT support team
4. Look for help icons (?) on the pages

**Remember**: These new features are designed to make your work easier and more organized. Take your time to learn them, and don't hesitate to ask for help!

---

*This guide covers the new v2 API features. For technical documentation, see the separate developer guide.*
