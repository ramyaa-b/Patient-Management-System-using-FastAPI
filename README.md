<h1>Patient Management System API</h1>

<body>This project is a lightweight, fully functional Patient Management System built using FastAPI.
It allows CRUD operations (Create, Read, Update, Delete) on patient records and computes health insights like BMI and health verdicts dynamically.</body>

<h2>Features</h2>

-View all patient records

-Add new patient data

-Edit existing patient information

-Delete patient records

-Sort patient list based on height, weight, or BMI

-Automatically compute BMI and classify patients into health categories: Underweight, Normal, or Obese

<h2>Concepts Used</h2>

FastAPI – to build RESTful API endpoints quickly and efficiently

Pydantic – for data validation and serialization

JSON – used as a lightweight, file-based database (patients.json)

CRUD operations – implemented with appropriate HTTP methods

BMI Calculation – body mass index calculated from height and weight

Dynamic Verdicts – BMI thresholds are used to determine health status

Data Persistence – patient data is saved and loaded from a JSON file

<h2>Software & Libraries Used</h2>

| Tool/Library    | Purpose                                 |
|----------------|------------------------------------------|
| Python          | Core programming language               |
| FastAPI         | Web framework for building APIs         |
| Pydantic        | Data parsing and validation             |
| Uvicorn         | ASGI server for running FastAPI apps    |
| JSON (built-in) | Used for storing and reading patient data |

<h2>Project Structure</h2>

├── main.py             # FastAPI application logic

├── patients.json       # JSON file storing patient records

└── README.md           # Documentation file 

<h2>Example Endpoints</h2>
GET / — Welcome message

GET /view — View all patients

POST /create — Add a new patient

PUT /edit/{id} — Update an existing patient

DELETE /delete/{id} — Remove a patient

GET /sort?sort_by=bmi&order=desc — Sort patients by BMI

<h2>Note</h2>

BMI = weight (kg) / height² (m²)

<h2>Health Verdicts:</h2>

BMI < 18.5 → Underweight

18.5 ≤ BMI < 30 → Normal

BMI ≥ 30 → Obese


Developed as a mini-project to demonstrate API design, data modeling, and CRUD operations using modern Python tools.

