# 🏥 Hospital Patient Data Analysis System

A professional **Hospital Patient Data Analysis System** developed as an academic web application using **Python, Flask, Pandas, Matplotlib, HTML, CSS, Bootstrap, and JavaScript**.

The system reads hospital patient data from CSV files, performs data cleaning and analysis, and presents useful statistics and visualizations through a responsive web dashboard.

> **Academic Project:** This application is designed for educational and demonstration purposes. It does not store or process real patient medical records.

---

## 📌 Project Overview

The **Hospital Patient Data Analysis System** helps users analyze patient information in a simple and visual way.

The application can:

- Read patient records from a CSV dataset
- Detect missing values
- Clean incomplete or invalid data
- Calculate patient statistics
- Analyze diseases and departments
- Analyze gender and age groups
- Search and filter patient records
- Upload a new CSV dataset
- Generate charts automatically
- Export cleaned patient data
- Display results through a professional dashboard

### Project Flow

```text
CSV Dataset
     ↓
Flask Application
     ↓
Pandas Data Processing
     ↓
Data Cleaning
     ↓
Data Analysis
     ↓
Matplotlib Visualization
     ↓
Web Dashboard
```

---

## ✨ Features

### 📊 Dashboard
- Total number of patients
- Average patient age
- Number of diseases
- Number of departments
- Missing-data summary
- Visual data representation

### 🧹 Data Cleaning
- Detects missing values
- Converts age values into numeric format
- Replaces missing age values with the average age
- Replaces empty text fields with `Unknown`
- Removes unnecessary spaces from text values

### 👨‍⚕️ Patient Management
- View patient records
- Search and filter patient information
- Display patient ID, name, age, gender, disease, and department

### 📈 Data Analysis
- Disease-wise patient analysis
- Department-wise patient analysis
- Gender-wise analysis
- Age-group analysis
- Average age calculation

### 📉 Data Visualization
The system automatically generates:

1. **Department Bar Chart**
2. **Disease Distribution Pie Chart**
3. **Age Distribution Histogram**

### 📤 CSV Upload
Users can upload a new patient CSV file through the web interface.

The uploaded file must contain:

```text
PatientID
Name
Age
Gender
Disease
Department
```

### 📥 Cleaned Data Export
The system provides an option to download the cleaned dataset as:

```text
cleaned_patients.csv
```

### 🔌 API
A summary API is available at:

```text
/api/summary
```

It returns key statistics such as:

- Total patients
- Average age
- Disease count
- Department count
- Missing-value count

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Flask | Backend web framework |
| Pandas | Data processing and analysis |
| Matplotlib | Graph generation |
| HTML5 | Web page structure |
| CSS3 | Styling |
| Bootstrap | Responsive UI design |
| JavaScript | Client-side interactions |
| Jinja2 | Flask template rendering |
| CSV | Dataset storage format |

---

## 📁 Project Structure

```text
Hospital_Patient_Data_Analysis_Professional/
│
├── app.py
├── patients.csv
├── requirements.txt
├── README.md
│
├── templates/
│   ├── base.html
│   ├── index.html
│   ├── dashboard.html
│   ├── patients.html
│   ├── analysis.html
│   └── upload.html
│
├── static/
│   ├── css/
│   │   └── style.css
│   │
│   ├── js/
│   │   └── app.js
│   │
│   └── graphs/
│       ├── department_bar.png
│       ├── disease_pie.png
│       └── age_histogram.png
│
└── uploads/
    └── cleaned_patients.csv
```

---

## 📋 Required CSV Format

The application expects the following columns:

```csv
PatientID,Name,Age,Gender,Disease,Department
```

### Example

```csv
P001,John,45,Male,Diabetes,General Medicine
P002,Anita,32,Female,Hypertension,Cardiology
P003,Ravi,60,Male,Arthritis,Orthopedics
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone <your-repository-url>
```

Move into the project directory:

```bash
cd Hospital_Patient_Data_Analysis_Professional
```

---

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

### Windows

```bash
venv\Scripts\activate
```

### Linux/macOS

```bash
source venv/bin/activate
```

---

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

The project requires:

```text
Flask
Pandas
Matplotlib
```

---

## ▶️ Run the Application

Start the Flask development server:

```bash
python app.py
```

The application will run locally at:

```text
http://127.0.0.1:5000
```

Open the address in your web browser.

---

## 🌐 Main Pages

| URL | Description |
|---|---|
| `/` | Home page |
| `/dashboard` | Analytics dashboard |
| `/patients` | Patient records |
| `/analysis` | Detailed analysis |
| `/upload` | Upload a CSV dataset |
| `/download-cleaned` | Download cleaned CSV |
| `/api/summary` | JSON summary API |

---

## 🔄 Data Processing Method

The application follows these main steps:

### Step 1 — Load Data
Patient information is loaded from `patients.csv` using Pandas.

### Step 2 — Validate Required Columns
The application checks for:

```text
PatientID
Name
Age
Gender
Disease
Department
```

### Step 3 — Clean Data
- Invalid age values are converted to missing values.
- Missing ages are replaced with the average age.
- Missing text values are replaced with `Unknown`.
- Extra spaces are removed.

### Step 4 — Analyze Data
The application calculates:

- Total patients
- Average age
- Disease counts
- Department counts
- Gender counts
- Age-group counts
- Missing-value statistics

### Step 5 — Generate Graphs
Matplotlib creates visualizations based on the cleaned data.

### Step 6 — Display Results
The processed information is displayed through Flask/Jinja2 web pages.

---

## 📊 Age Groups

Patients are categorized into the following groups:

```text
0–17
18–30
31–45
46–60
61+
```

This helps understand the distribution of patients across different age ranges.

---

## 🔐 Security / Academic Scope

This project is intended for **local academic demonstration**.

It should not be deployed with real patient information without implementing appropriate healthcare data security, authentication, authorization, encryption, auditing, and applicable legal/privacy requirements.

Before production use, the Flask development configuration and hard-coded demo secret should also be replaced with secure production configuration.

---

## 🚀 Future Enhancements

Possible future improvements include:

- User authentication and role-based access
- MySQL/PostgreSQL database integration
- Advanced patient search
- Date-wise analysis
- Doctor-wise analysis
- Hospital admission/discharge analysis
- Interactive charts using Chart.js
- PDF report generation
- Excel report generation
- Machine-learning based prediction
- Cloud deployment
- Secure database storage
- Advanced filtering and pagination

---

## 🎓 Academic Objectives

The main objectives of this project are:

1. To understand hospital patient datasets.
2. To perform data cleaning using Pandas.
3. To analyze patient information using Python.
4. To visualize data using Matplotlib.
5. To develop a web application using Flask.
6. To present analytical results through a dashboard.
7. To understand CSV-based data processing and reporting.

---

## 👥 Project Type

**Project Category:** Academic / Educational Web Application

**Domain:** Healthcare Data Analysis

**Backend:** Python + Flask

**Data Analysis:** Pandas

**Visualization:** Matplotlib

**Frontend:** HTML, CSS, Bootstrap, JavaScript

**Data Source:** CSV

---

## 📄 License

This project is created for academic and educational purposes.

You may modify and extend the project for learning and demonstration purposes.

---

## ⭐ Conclusion

The **Hospital Patient Data Analysis System** provides a simple and professional way to process, analyze, and visualize hospital patient data.

By combining **Flask for web development, Pandas for data analysis, and Matplotlib for visualization**, the system demonstrates how raw CSV data can be transformed into meaningful analytical information through a web-based dashboard.
