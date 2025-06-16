## Project Overview: Coursework for Lapin AMK, Edistynyt Tiedonhallinta (Lapland UAS, Advanced Data Management) through Open UAS studies

Follow the steps below to set up and run the system:

### 1.  Import Databases
- Use **phpMyAdmin** to import the OLAP and OLTP SQL files:
  - Navigate to **Import → File to import**
  - Use files from the **`Databases/`** folder

### 2. Populate OLTP with Faker Data
- Run `main3.py` located in the **`Insert Faker Data/`** folder
- This will insert sample data into the OLTP database

### 3. Run ETL Process
- Run `main2.py` located in the **`ETL/`** folder
- This extracts data from OLTP and loads it into OLAP

### 4. Launch REST API
- Run `main.py` in the **`REST/`** folder
- This launches a REST API to perform predefined queries on the OLAP data


## Dependency Management

If you encounter any errors during execution, it's likely due to missing or incompatible dependencies. To ensure stability, navigate to each folder separately: 



```bash
pip install -r requirements.txt
pip install -r requirements2.txt
pip install -r requirements3.txt
