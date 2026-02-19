# API Documentation

The backend exposes internal routes handled by Flask to manage inventory operations.

## Routes

### GET /
- Displays the inventory dashboard
- Shows all inventory items

### GET /add
- Displays the form to add a new inventory item

### POST /add
- Accepts form data
- Adds a new item to the inventory database

### GET /restock
- Displays restock recommendations
- Uses intelligent agent logic to compute restocking quantities

## Internal Logic

The intelligent agent is invoked internally when the restock route is accessed. No external API calls are required.

The system is designed to be simple and self-contained.
