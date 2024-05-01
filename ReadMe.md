#Vendor Management System
The Vendor Management System is a Django-based application for managing vendor profiles, tracking purchase orders, and calculating vendor performance metrics.

## Setup Instructions
1. Clone the repository:
bash
Copy code
git clone https://github.com/yourusername/vendor-management-system.git
Navigate to the project directory:
bash
Copy code
cd vendor-management-system
Create a virtual environment:
bash
Copy code
python -m venv venv
Activate the virtual environment:
On Windows:
bash
Copy code
venv\Scripts\activate
On macOS and Linux:
bash
Copy code
source venv/bin/activate
Install the dependencies:
bash
Copy code
pip install -r requirements.txt
Apply migrations:
bash
Copy code
python manage.py migrate
Run the development server:
bash
Copy code
python manage.py runserver
Using the API Endpoints
Vendor Endpoints
List/Create Vendors:
URL: /api/vendors/
Method: GET (List), POST (Create)
Description: Retrieve a list of vendors or create a new vendor.
Parameters: None (for GET), JSON data (for POST)
Retrieve/Update/Delete Vendor:
URL: /api/vendors/{vendor_id}/
Method: GET (Retrieve), PUT (Update), DELETE (Delete)
Description: Retrieve, update, or delete a specific vendor by ID.
Parameters: vendor_id (in the URL)
Vendor Performance Metrics:
URL: /api/vendors/{vendor_id}/performance/
Method: GET
Description: Retrieve the performance metrics for a specific vendor.
Parameters: vendor_id (in the URL)
Purchase Order Endpoints
List/Create Purchase Orders:
URL: /api/purchase_orders/
Method: GET (List), POST (Create)
Description: Retrieve a list of purchase orders or create a new purchase order.
Parameters: None (for GET), JSON data (for POST)
Retrieve/Update/Delete Purchase Order:
URL: /api/purchase_orders/{po_id}/
Method: GET (Retrieve), PUT (Update), DELETE (Delete)
Description: Retrieve, update, or delete a specific purchase order by ID.
Parameters: po_id (in the URL)

 This assignment tests your ability to create a functional Django-based system for vendor
 management, integrating aspects of data handling, API development, and basic performance
 metric calculations
