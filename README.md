
Smart Inventory Management System
A Python and Streamlit mini-project for inventory overview, expiry monitoring, defect analysis and simple short-term demand estimation.

Features
Dashboard with product count, stock quantity, expiry indicators and defect totals.
Inventory editing and product addition.
Expired, near-expiry (within 30 days) and safe-stock views.
Defect count and defect percentage analysis.
Seven-day demand estimate using Scikit-learn Linear Regression.
Inventory and sales CSV upload/download.
Technology stack
Python, Streamlit, Pandas, NumPy, Plotly and Scikit-learn.

Run locally
Install Python 3.9 or later.
Open a terminal in this repository folder.
Create and activate a virtual environment (recommended):
Windows: py -m venv .venv
Windows CMD: .venv\Scripts\activate
Install dependencies: py -m pip install -r requirements.txt
Start the app: py -m streamlit run app.py
Open the local URL printed by Streamlit (normally http://localhost:8501).
CSV formats
Inventory CSV
Required headers: item,category,quantity,unit_price,expiry_date,defect_count

Date format: YYYY-MM-DD. See data/sample_inventory.csv.

Sales history CSV
Required headers: date,item,demand

Date format: YYYY-MM-DD. See data/sample_sales.csv.

Important implementation notes
The application begins with demonstration data generated in memory.
Uploaded and edited data is held in Streamlit session state while the app session is active. This version does not provide permanent database storage.
Demand estimates are generated from the selected product's available historical demand values using a basic Linear Regression model. They are illustrative estimates, not guaranteed forecasts.
This version does not connect to AWS or implement cloud storage, authentication, role-based access, or enterprise security controls.
Screenshots
Add your genuine screenshots from the running application to the screenshots/ folder. Suggested captures:

Dashboard
Inventory Management
Expiry Monitoring
Defect Analysis
Demand Prediction
CSV Upload/Download
Repository structure
SmartInventoryProject/
├── app.py
├── requirements.txt
├── README.md
├── REPORT.md
├── data/
│   ├── sample_inventory.csv
│   └── sample_sales.csv
└── screenshots/
Academic integrity
Replace generic report details with your actual name, register number, department, institution, guide and academic year. Include only screenshots and test results you personally verified.

