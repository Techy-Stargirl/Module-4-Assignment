# Module-4-Assignment - Netflix Data Analysis Project
This project analyzes Netflix shows and movies data to gain insights into content trends, ratings distribution, and popular genres.

## Prerequisites

Before running the code, ensure you have the following installed:

* **Python 3.x:** [https://www.python.org/downloads/](https://www.python.org/downloads/)
* **Required Python Libraries:**
    * `pandas`
    * `numpy`
    * `matplotlib`
    * `seaborn`
    * `zipfile`
    * `rpy2` (if you want to run the R integration part)
* **R** (if you want to run the R integration part): [https://www.r-project.org/](https://www.r-project.org/)

## Installation

1.  **Clone the repository (if applicable):**
    ```bash
    # If you have the code in a git repository. Otherwise, download the files.
    git clone [repository URL]
    ```

2.  **Install Python Libraries:**
    Open your terminal or command prompt and run:
    ```bash
    pip install pandas numpy matplotlib seaborn rpy2
    ```

3.  **Install R (if needed):**
    * Download and install R from the official website.
    * Ensure R is added to your system's PATH.

## Data Preparation

1.  Download the `netflix_data.zip` file and place it in the `Downloads` folder of the current user.
2.  The Python script will automatically unzip the file and rename the extracted CSV.

## Running the Code

1.  **Navigate to the project directory:**
    Open your terminal or command prompt and use the `cd` command to navigate to the directory where you saved the Python script (e.g., `netflix_analysis.py`).
2.  **Run the Python script:**
    ```bash
    python netflix_analysis.py
    ```
    or, if you are using python 3 and have python 2 installed as well.
    ```bash
    python3 netflix_analysis.py
    ```

## Output

The script will produce the following output:

* **Console Output:**
    * Initial and final missing value counts.
    * Data description and information.
    * Value counts of the 'type' column.
    * Statistical analysis of the 'release_year' column.
    * If R integration is successful, a message stating that the chart was created.
    * If R integration fails, a message explaining why.
      
* **Visualizations:**
    * "Top 10 Most Watched Genres" bar plot (`Top_10_Most_Watched_Genres.png`).
    * "Ratings Distribution" count plot (`Ratings_Distribution.png`).
    * "ratings_distribution_r.png" if the R integration is successful.

## Error Correction and Improvements

1.  **File Naming Conflict:**
    * The original code had a potential issue where renaming the extracted file could fail if a file with the new name already existed.
    * This code now overwrites the file if it exists.
2.  **File Path:**
    * The file path has been kept as the original path. If the file is placed in a different location, the file path will have to be changed within the python file.

## Note

* If `rpy2` is not installed, the R integration part of the code will be skipped, and the script will continue to run without it.
* Ensure that the `netflix_data.zip` file is in the specified directory before running the script.
* The matplotlib gra
