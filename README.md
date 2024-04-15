# project-feed-conversion-ratio-optimization
The primary goal of this project was to gain practical experience with FCR calculation and its role in poultry performance. By analyzing a sample dataset, I aimed to explore how data analysis can help by alleviate the feed calculation process for better FCR. 
This project provides a simple Python script to calculate Feed Conversion Ratio (FCR) for a flock of birds and suggest their next week's feed intake based on weight gain.

**Requirements:**

* Python 3 (tested with version 3.8)
* pandas library (`pip install pandas`)
* NumPy library (`pip install numpy`)

**Data Format:**

The script expects your data in a comma-separated values (CSV) file. The file should have the following columns:

* Bird ID (unique identifier for each bird)
* Age (in weeks) - Optional (not used in the current FCR calculation)
* Breed (Optional) - Not used in the current FCR calculation, but might be useful for future improvements.
* Initial Weight (grams)
* Final Weight (grams)
* Weekly Feed Intake (grams)

**How to Use:**

1. **Save your data:** Prepare your data in a CSV file with the required columns. 
2. **Clone or Download the Repository:** If you downloaded the code from GitHub, unzip the folder. If you cloned the repository using Git, navigate to the project directory using your terminal.
3. **Run the Script:** Open a terminal or command prompt in the project directory. Execute the following command, replacing `data.csv` with the actual filename of your data file:

```
python fcr_analysis.py data.csv
```

4. **Output:** The script will generate a new CSV file named `fcr_results.csv` in the same directory. This file will contain the following columns:

* Bird ID
* Weight Gain (Final Weight - Initial Weight)
* FCR (Weekly Feed Intake / Weight Gain)
* Suggested Feed Intake (based on assumed average daily gain)

**Note:** The suggested feed intake is an estimate and may need adjustments based on factors like breed, age, and individual bird differences. It's recommended to consult a poultry expert for breed-specific recommendations.

**Adding Features:**

This is a basic script with potential for further development. Here are some ideas for future improvements:

* **Incorporate Breed Data:**  Include breed information in the analysis to account for breed-specific variations in FCR.
* **Refine Feed Intake Suggestions:** Use breed-specific average daily gain values for more accurate feed intake suggestions.
* **Data Visualization:** Create charts or graphs to visualize trends in weight gain, FCR, or feed intake across different birds.
* **Error Handling:** Implement error handling to gracefully handle potential issues like missing data or invalid file formats.

**Contributing:**

If you'd like to contribute to the project, feel free to fork the repository on GitHub and submit pull requests with your improvements or bug fixes.
