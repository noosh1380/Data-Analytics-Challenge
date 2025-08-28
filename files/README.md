# Customer Segmentation Analysis

## Project Structure  
The repository is organized as follows:  

```
project_root/
│
├── data/
│   ├── customer_transactions.csv      # Raw dataset
│   ├── cleaned_data.csv               # Preprocessed dataset
│
├── files/
│   └── README.md                      # This file
│
├── notebooks/
│   └── Customer_Segmentation_Analysis.ipynb   # Jupyter Notebook with full code, analysis, visualizations, and summary
```

---

## Setup & Run Instructions  

1. **Clone the repository** (or download the files).  
   
2. **Create a virtual environment** (Python 3.11 was used in development):  
   ```bash
   python3.11 -m venv venv
   source venv/bin/activate   # On macOS/Linux
   venv\Scripts\activate      # On Windows
   ```

3. **Install dependencies**:  
   ```bash
   pip install pandas numpy seaborn matplotlib scikit-learn jupyter
   ```

4. **Run Jupyter Notebook**:  
   ```bash
   jupyter notebook
   ```

5. **Navigate to the notebook** in the `notebooks/` folder and open:  
   ```
   notebooks/Customer_Segmentation_Analysis.ipynb
   ```

6. **Important note**:  
   - The Jupyter Notebook assumes that the working directory is the notebooks/ folder hence it loads the dataset using a relative path to the parent directory:  
     ```python
     df = pd.read_csv("../data/customer_transactions.csv")
     ```

---

## Analysis & Assumptions  

- **Clustering Method**:  
  - K-Means clustering was used.  
  - The chosen number of clusters (`k`) is **2**.  

- **Data Assumptions**:  
  - `CustomerID`, `Age`, `Annual Income (k$)`, `Spending Score (1-100)`, `Purchase Frequency`, and `Total Sales` are treated as integers.  
  - `Gender` is assumed to have only two categories: **Male** and **Female**.  

- **Data Files**:  
  - The raw dataset is stored as `customer_transactions.csv` in the `data/` folder.  
  - A cleaned version of the dataset is also provided as `cleaned_data.csv`.  

- **Reporting**:  
  - As per the project instructions, no separate summary report (`report.md` or `report.pdf`) was created.  
  - The full **code, analysis, visualizations, and written summary** are documented directly in the Jupyter Notebook.  

---

## Requirements  

- Python 3.11  
- Packages:  
  - `pandas`  
  - `numpy`  
  - `seaborn`  
  - `matplotlib`  
  - `scikit-learn`  
  - `jupyter`  
