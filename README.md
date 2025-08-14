💻 Laptop Pricing Data Analysis & Cleaning Project
🔍 Overview
This project demonstrates data cleaning, preprocessing, and exploratory analysis on a laptop pricing dataset. The goal was to handle missing values, normalize features, convert units, and analyze pricing trends.

📌 Skills Demonstrated
✅ Data Cleaning – Handling missing values (NaN, ?), dropping unnecessary columns.
✅ Feature Engineering – Unit conversion (kg → pounds, cm → inches), normalization.
✅ Data Preprocessing – One-hot encoding (Screen type).
✅ Exploratory Data Analysis (EDA) – Descriptive stats, price binning, bar plots.
✅ Python Libraries Used – Pandas, NumPy, Matplotlib.

📂 Dataset
Source: Custom laptop pricing dataset (laptop_pricing_dataset_mod1.csv)
Features:

Numerical: Price, CPU_frequency, RAM_GB, Storage_GB_SSD, etc.

Categorical: Manufacturer, Category, Screen, OS, etc.

🔧 Data Processing Steps
Handled Missing Values

Replaced ? with NaN.

Filled missing Weight_kg with mean value.

Filled missing Screen_Size_cm with the most frequent value (39.624 cm → ~15.6 inches).

Unit Conversions & Normalization

Converted Screen_Size_cm → Screen_Size_inch (divided by 2.54).

Converted Weight_kg → Weight_pounds (multiplied by 2.205).

Normalized CPU_frequency (divided by max value).

Price Binning

Categorized Price into Low, Medium, High ranges.

Visualized distribution with a bar plot.

Categorical Data Encoding

One-hot encoded Screen type (Full HD, IPS Panel).

Data Export

Cleaned dataset ready for further analysis.

📊 Key Findings
✔ Most Common Screen Size: ~15.6 inches (after conversion).
✔ Weight Distribution: Average laptop weight ≈ X pounds (after conversion).
✔ Price Categories:

Low: $X - $Y

Medium: $Y - $Z

High: $Z+

✔ Missing Data Handling:

Weight_kg had missing values → filled with mean.

Screen_Size_cm had missing values → filled with mode.

📂 Project Structure
text
laptop-data-analysis/  
├── data/  
│   ├── laptop_pricing_dataset_base.csv   # Raw dataset  
│   └── laptop_pricing_dataset_mod1.csv   # Modified dataset  
├── cleaned_laptop_data.csv               # Processed data (optional export)  
└── README.md                             # Project documentation  
