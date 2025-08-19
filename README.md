# Supplier Correlation Analysis - OptimalFlow

This repository contains the correlation analysis outputs for the supply chain dataset provided by the client.

**Contact / student email:** 24f2005647@ds.study.iitm.ac.in

Files included:
- `correlation.csv` - Pearson correlation matrix for selected supply chain metrics
- `heatmap.png` - Heatmap (red=low, white=mid, green=high) visualizing correlations

Quick findings (top absolute correlations):
- Supplier_Lead_Time ↔ Cost_Per_Unit: 0.957 (strong positive)
- Supplier_Lead_Time ↔ Delivery_Performance: -0.935 (strong negative)
- Delivery_Performance ↔ Cost_Per_Unit: -0.929 (strong negative)
- Supplier_Lead_Time ↔ Order_Frequency: -0.891 (strong negative)
- Order_Frequency ↔ Cost_Per_Unit: -0.888 (strong negative)

How to reproduce (Excel):
- Enable Analysis ToolPak (File → Options → Add-Ins → Analysis ToolPak).
- Data → Data Analysis → Correlation; select all five columns, check "Labels in first row", output to new worksheet.
- Apply Conditional Formatting → Color Scales → 3-Color Scale (Red / White / Green) to the numeric cells.
