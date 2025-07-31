# Salesforce CRM Project

A Salesforce CRM application built with Apex triggers for order management and inventory tracking.

## Project Overview

This project implements a comprehensive CRM solution with the following features:

- **Order Management**: Automated order total calculations
- **Inventory Tracking**: Real-time stock deduction and monitoring  
- **Customer Management**: Complete customer relationship management
- **Low Stock Alerts**: Automated alerts for inventory management
- **Loyalty Program**: Customer loyalty program implementation

## Features

### 1. Order Total Calculation
- Automatically calculates order totals based on product price and quantity
- Implements real-time pricing updates

### 2. Stock Management
- Automatic stock deduction when orders are confirmed
- Real-time inventory tracking
- Low stock alert system

### 3. Customer Portal
- Customer order tracking
- Order confirmation emails
- Loyalty program integration

## Technical Implementation

### Apex Triggers

#### OrderTotalTrigger
- **Purpose**: Calculates total amount for orders
- **Events**: Before insert, before update
- **Logic**: Multiplies quantity by product price to determine total amount

#### StockDetectionTrigger  
- **Purpose**: Manages inventory levels
- **Events**: After insert, after update
- **Logic**: Deducts stock quantity when orders are confirmed

### Custom Objects
- `HandsMen_Order__c` - Order management
- `HandsMen_Product__c` - Product catalog
- `Inventory__c` - Stock management

## Project Structure

```
├── code/
│   ├── OrderTotalTrigger.txt    # Order total calculation trigger
│   └── StockDetectionTrigger.txt # Stock deduction trigger
├── screenshots/
│   ├── customers.png            # Customer management interface
│   ├── inventory.png            # Inventory dashboard
│   ├── orders.png              # Order management view
│   ├── product.png             # Product catalog
│   └── ... (additional UI screenshots)
├── demo.mp4                    # Project demonstration video
└── README.md                   # Project documentation
```

## Setup Instructions

1. **Salesforce Org Setup**
   - Create a Salesforce Developer Org
   - Set up custom objects and fields as required

2. **Deploy Triggers**
   - Deploy the Apex triggers using Salesforce CLI or Developer Console
   - Ensure proper test coverage before deployment

3. **Configure Custom Objects**
   - Create the custom objects: `HandsMen_Order__c`, `HandsMen_Product__c`, `Inventory__c`
   - Set up required fields and relationships

## Screenshots

The `screenshots/` folder contains visual documentation of:
- Customer management interface
- Inventory tracking dashboard
- Order processing workflow
- Low stock alert system
- Loyalty program features
- Order confirmation flows

## Demo

Watch the complete project demonstration in `demo.mp4` to see all features in action.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add appropriate test coverage
5. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Contact

For questions or support, please open an issue in this repository.
