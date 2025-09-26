# Telecom ETL Project (SSIS)

## 📌 Overview  
This project demonstrates a **Telecom ETL (Extract, Transform, Load)** pipeline built using **SQL Server Integration Services (SSIS)**.  
The solution extracts raw CSV data, cleans and transforms it, and loads it into a structured SQL Server database optimized for analytics and reporting.  

## 📂 Project Structure
```
Project ETL SSIS/
│── ETL - Telecom.docx           # Project documentation
│── Source Files/                # Sample raw data files (CSV)
│── SQL Qureries/                # SQL scripts for database setup
│── Telecome ETL SSIS/           # SSIS project files
│   ├── Package.dtsx             # Main SSIS package
│   ├── Telecome ETL SSIS.dtproj # SSIS project configuration
│   ├── Telecome ETL SSIS.sln    # Visual Studio solution
│── .git/                        # Git version control metadata
```

## ⚙️ Features
- **Data Extraction** from multiple CSV batch files.  
- **Data Transformation**:
  - Handling null values  
  - Data type conversions  
  - Business rules enforcement  
- **Data Loading** into SQL Server:
  - Fact tables (transactions)  
  - Dimension tables (IMSI, errors, etc.)  

## 🚀 Getting Started

### 1. Requirements
- SQL Server (2019 or later recommended)  
- SQL Server Data Tools (SSDT) or Visual Studio with SSIS extension  
- Git (optional, for version control)  

### 2. Setup
1. Clone or extract this repository:  
   ```bash
   git clone <repo-url>
   ```
2. Create a SQL Server database using the scripts in **`SQL Qureries/`**:  
   - `01. Create database.sql`  
   - `02. Create fact transaction table.sql`  
   - `04. Create dim imsi.sql`  
   - etc.  
3. Open **`Telecome ETL SSIS.sln`** in Visual Studio.  
4. Configure connection managers (adjust to your local SQL Server & file paths).  
5. Run **`Package.dtsx`** to execute the ETL pipeline.  

### 3. Input Data
- CSV files are located in `Source Files/`.  
- They represent raw telecom transaction data, split across batches.  

### 4. Output
- Cleaned and transformed data loaded into SQL Server tables for reporting and analytics.  

## 📖 Documentation
See **`ETL - Telecom.docx`** for detailed explanation of design, transformations, and business rules.  

## 👨‍💻 Author
Developed as part of a **Telecom Data Engineering ETL Project** using **SSIS & SQL Server**.  

