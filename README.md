# ECE 2112: Advanced Computer Programming and Algorithms

**Experiment 3: Python Data Analysis (Pandas) || Programmed by: Buño, James Patrick T.**

This repository contains the Jupyter Notebook solution for Experiment 3, demonstrating data loading, positional and label-based indexing, Boolean filtering, and DataFrame subsetting using Pandas on the `cars.csv` dataset. As per the laboratory instructions, no external Python libraries other than Pandas were used.

## A. Positional and Label-Based Slicing
Loads `cars.csv` into a DataFrame named `cars`, displays its shape and column names, and extracts rows 6 through 10[cite: 4, 5]. Displays the columns `Model`, `mpg`, `cyl`, `hp`, and `gear` for this subset.
* **Technique Used:** Shape inspection (`cars.shape`), column listing (`list(cars.columns)`), positional row slicing with `.iloc`, and label-based column indexing with `.loc"`.

## B. Model Lookup
Uses Boolean indexing on the `Model` column to retrieve the full row record for `Toyota Corolla` (stored in `toyota`) and selected attributes (`Model`, `mpg`, `hp`, `wt`) for `Pontiac Firebird` (stored in `pontiac`).
* **Technique Used:** Conditional Boolean indexing (`cars['Model'] == '...'`) and label-based subset selection (`.loc`) without hardcoding row indices.

## C. Multi-Model Subsetting[cite:
Extracts records for three specific models (`Datsun 710`, `Lotus Europa`, and `Ferrari Dino`) into a DataFrame named `selected_cars` while retaining only `Model`, `mpg`, `cyl`, `hp`, and `gear`.
* **Technique Used:** Multi-value filtering using `.isin()`, column label subsetting, and dimensional verification (`.shape`) confirming a 3×5 output.

---

## 📥 Access the Notebook

To view the full code and executed test cells showing all requested outputs, open the Jupyter Notebook file in this repository:
[**EXPERIMENT 3 PYTHON DATA ANALYSIS (PANDAS).ipynb**](./EXPERIMENT%203%20PYTHON%20DATA%20ANALYSIS%20(PANDAS).ipynb)
