# System Architecture

The Inventory Management System follows a modular and layered architecture to ensure clarity, scalability, and maintainability.

## Architectural Components

### 1. Presentation Layer
- Built using HTML, CSS, and Jinja2 templates
- Responsible for displaying inventory data, forms, and restock recommendations
- Provides a clean and user-friendly interface

### 2. Application Layer
- Implemented using Flask (Python)
- Handles routing, request processing, and response rendering
- Acts as the bridge between the frontend and backend logic

### 3. Intelligent Agent Layer
- Implemented as a separate module
- Analyzes inventory data
- Applies decision-making logic to recommend restocking quantities

### 4. Data Layer
- Uses SQLite as the database
- Stores inventory items, quantities, and minimum thresholds
- Ensures persistent data storage

## Data Flow

1. User interacts with the web interface
2. Requests are sent to the Flask backend
3. Inventory data is retrieved from the database
4. Intelligent agent evaluates stock levels
5. Restock recommendations are generated
6. Results are displayed to the user
