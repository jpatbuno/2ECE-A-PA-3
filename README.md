# ECE 2112: Advanced Computer Programming and Algorithms[cite: 5]

**Experiment 3: Python Data Analysis (Pandas) || Programmed by: Buño, James Patrick T.**[cite: 4, 5]

This repository contains the Jupyter Notebook solution for Experiment 3, demonstrating data loading, positional and label-based indexing, Boolean filtering, and DataFrame subsetting using Pandas on the `cars.csv` dataset[cite: 4, 5]. As per the laboratory instructions, no external Python libraries other than Pandas were used[cite: 5].

## A. Positional and Label-Based Slicing[cite: 4, 5]
Loads `cars.csv` into a DataFrame named `cars`, displays its shape and column names, and extracts rows 6 through 10[cite: 4, 5]. Displays the columns `Model`, `mpg`, `cyl`, `hp`, and `gear` for this subset[cite: 4, 5].
* **Technique Used:** Shape inspection (`cars.shape`), column listing (`list(cars.columns)`), positional row slicing with `.iloc`, and label-based column indexing with `.loc`[cite: 4, 5].

## B. Model Lookup[cite: 4, 5]
Uses Boolean indexing on the `Model` column to retrieve the full row record for `Toyota Corolla` (stored in `toyota`) and selected attributes (`Model`, `mpg`, `hp`, `wt`) for `Pontiac Firebird` (stored in `pontiac`)[cite: 4, 5].
* **Technique Used:** Conditional Boolean indexing (`cars['Model'] == '...'`) and label-based subset selection (`.loc`) without hardcoding row indices[cite: 4, 5].

## C. Multi-Model Subsetting[cite: 4, 5]
Extracts records for three specific models (`Datsun 710`, `Lotus Europa`, and `Ferrari Dino`) into a DataFrame named `selected_cars` while retaining only `Model`, `mpg`, `cyl`, `hp`, and `gear`[cite: 4, 5].
* **Technique Used:** Multi-value filtering using `.isin()`, column label subsetting, and dimensional verification (`.shape`) confirming a 3×5 output[cite: 5].

---

## 📥 Access the Notebook

To view the full code and executed test cells showing all requested outputs, open the Jupyter Notebook file in this repository:
[**EXPERIMENT 3 PYTHON DATA ANALYSIS (PANDAS).ipynb**](./EXPERIMENT%203%20PYTHON%20DATA%20ANALYSIS%20(PANDAS).ipynb)[cite: 4]
