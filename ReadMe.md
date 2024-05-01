# Vendor Management System
The Vendor Management System is a Django-based application for managing vendor profiles, tracking purchase orders, and calculating vendor performance metrics.

## Setup Instructions
### 1. Clone the repository:
```bash 
 git clone https://github.com/yourusername/vendor-management-system.git
```
### 2. Navigate to the project directory:
```bash
 cd vendor-management-system
```
### 3. Create a virtual environment:
```bash
 python -m venv venv
```
### 4. Activate the virtual environment:
On Windows:
```bash
 venv\Scripts\activate
```
On macOS and Linux:
```bash
 source venv/bin/activate
```
### 5. Install the dependencies:
```bash
 pip install -r requirements.txt
```
### 6. Apply migrations:
```bash
 python manage.py migrate
```
### 7. Run the development server:
```bash
 python manage.py runserver
```
## Using the API Endpoints
### Vendor Endpoints

- [x] List/Create Vendors:
   - URL: /api/vendors/ 
   - Method: GET (List), POST (Create)
   - Description: Retrieve a list of vendors or create a new vendor.
   - Parameters: None (for GET), JSON data (for POST)

- [X] Retrieve/Update/Delete Vendor:
   - URL: /api/vendors/{vendor_id}/
   - Method: GET (Retrieve), PUT (Update), DELETE (Delete)
   - Description: Retrieve, update, or delete a specific vendor by ID.
   - Parameters: vendor_id (in the URL)

- [x] Vendor Performance Metrics:
   - URL: /api/vendors/{vendor_id}/performance/
   - Method: GET
   - Description: Retrieve the performance metrics for a specific vendor.
   - Parameters: vendor_id (in the URL)
### Purchase Order Endpoints
- [x] List/Create Purchase Orders:
   - URL: /api/purchase_orders/
   - Method: GET (List), POST (Create)
   - Description: Retrieve a list of purchase orders or create a new purchase order.
   - Parameters: None (for GET), JSON data (for POST)
- [x] Retrieve/Update/Delete Purchase Order:
   - URL: /api/purchase_orders/{po_id}/
   - Method: GET (Retrieve), PUT (Update), DELETE (Delete)
   - Description: Retrieve, update, or delete a specific purchase order by ID.
   - Parameters: po_id (in the URL)

