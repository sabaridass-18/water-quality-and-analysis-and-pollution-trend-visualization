# Water Quality Analysis and Pollution trend Visualization

## Problem Statement
Analyze water-quality measurements over time and across locations to explore possible pollution trends. The project focuses on pH, dissolved oxygen, turbidity, total dissolved solids (TDS), nitrate, lead, and temperature.

## Dataset Source and Description
- **Source:** The notebook loads an Excel workbook uploaded by the user in Google Colab. The original publisher/source of the workbook is not specified in the notebook.
- **Required workbook sheets:** `Original_Dataset` and `Cleaned_Dataset`.
- **Fields used:** `Date`, `Location`, `pH`, `Dissolved_Oxygen_mg_L`, `Turbidity_NTU`, `TDS_mg_L`, `Nitrate_mg_L`, `Lead_mg_L`, and `Temperature_C`.

Keep the Excel workbook used by the notebook available when running the project.

## Steps Followed

1. **Import libraries** — use Pandas for data handling, Matplotlib for charts, and Seaborn for the correlation heatmap.
2. **Upload and load data** — upload the Excel workbook and read the `Original_Dataset` and `Cleaned_Dataset` sheets.
3. **Prepare data** — convert the `Date` column to datetime format.
4. **Check missing values** — compare missing-value counts in the original and cleaned datasets.
5. **Analyze trends over time** — plot turbidity, nitrate, lead, pH, and dissolved oxygen against date.
6. **Compare locations** — calculate location-wise averages for turbidity, nitrate, and lead and display them in a bar chart.
7. **Study relationships** — calculate correlations among pH, dissolved oxygen, turbidity, TDS, nitrate, lead, and temperature, then visualize them with a heatmap.

## Key Findings
The notebook creates charts to help investigate:
- Changes in turbidity, nitrate, and lead concentrations over time.
- Changes in pH and dissolved oxygen over time.
- Differences in average turbidity, nitrate, and lead between locations.
- Correlations among the selected water-quality parameters.
- Missing-value counts before and after cleaning.

**Note:** The notebook file contains the analysis code but does not include the dataset values or saved chart outputs. Therefore, specific trends, highest-pollution locations, and correlation strengths should be reported only after running the notebook with the actual Excel workbook.

## How to Run the Project

1. Open the notebook in [Google Colab](https://colab.research.google.com/) or a Jupyter environment.
2. Ensure the required Python libraries are available:
   - `pandas`
   - `matplotlib`
   - `seaborn`
   - `openpyxl` (for reading Excel files)
3. Run the notebook cells in order.
4. When prompted, upload the Excel workbook containing `Original_Dataset` and `Cleaned_Dataset` sheets.
5. Review the missing-value summaries and generated charts.

The notebook currently imports `google.colab.files`, so the upload cell is intended for Google Colab. In a local Jupyter environment, replace that upload step with a local file path.

## Charts and Visualizations
The notebook generates the following visualizations:

- Water Turbidity Trend Over Time
- Nitrate Pollution Trend Over Time
- Lead Concentration Trend
- Water Pollution Indicators by Location
- Correlation Between Water Quality Parameters (heatmap)
- pH Level of Water Over Time
- Dissolved Oxygen Trend Over Time

After running the notebook, screenshots of the generated charts can be added here, for example:

```markdown
![Water Turbidity Trend](images/turbidity_trend.png)
![Nitrate Pollution Trend](images/nitrate_trend.png)
![Correlation Heatmap](images/correlation_heatmap.png)
```

## Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Google Colab / Jupyter Notebook
