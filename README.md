# 📦 Inventory Management System

A comprehensive MySQL database system designed for efficient product and inventory management. This system supports detailed product tracking with variations, attributes, and brand management.

## 📋 Features

- Product management with brand and category organization
- Detailed product variations (size and color combinations)
- Flexible attribute system for product specifications
- Product image management
- Stock quantity tracking
- Price management for different variations

## 🚀 Setup Instructions

1. **Database Setup**

   ```sql
   -- Import the database schema
   mysql -u your_username -p < inventory.sql
   ```

2. **System Requirements**
   - MySQL 8.0 or higher
   - Sufficient storage for product images
   - Basic understanding of relational databases

## 📊 Database Structure

The system uses a normalized database design with the following main tables:

### Core Tables

- `brand` - Stores brand information
- `product_category` - Product classification categories
- `products` - Main product information with brand and category references

### Variation Management

- `colors` - Available color options
- `size_category` - Categories of sizes (e.g., clothing, shoes)
- `size_option` - Specific size options within categories
- `product_item` - Individual product items with specific variations
- `product_variation` - Product variation combinations

### Additional Features

- `product_image` - Product image management
- `attributes_category` - Categories for product attributes
- `attributes_type` - Types of attributes with data types
- `product_attribute` - Product-specific attributes

## 🔑 Key Relationships

- Products are linked to brands and categories
- Product items combine products with specific color and size variations
- Attributes can be assigned to products with specific data types
- Images can be associated with products
- Size options are organized by categories

## 🔧 Maintenance

Regular maintenance tasks:

- Daily inventory reconciliation
- Weekly stock level reports
- Monthly inventory audits
- Quarterly database optimization
## ERD
![Inventory_management_db](https://github.com/Mochez01/Inventory_management_db/blob/master/ERD.png)
