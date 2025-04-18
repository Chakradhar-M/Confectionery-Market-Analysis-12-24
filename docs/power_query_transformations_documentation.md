
###  Power Query Transformations

This Power Query transformation flow prepares raw confectionery sales data for market share and performance analysis. The goal is to clean, structure, and enhance the data to enable accurate and insightful reporting.


### 📋 **Transformation Steps**

1. **Source Data Connection**  
   - Connected to an Excel file named `dataset_fp20_nov_24.xlsx` and loaded the `Data` sheet.

2. **Promote Headers**  
   - Promoted the first row as column headers to structure the data table.

3. **Change Data Types**  
   - Assigned appropriate data types to all columns (e.g., year as whole number, text for categorical values, etc.).

4. **Rename Column (EUR Column)**  
   - Renamed `"SALES VOLUME  in EUR"` to `"SALES VOLUME  IN EUR"` to correct inconsistent spacing.

5. **Create Month Number Column**  
   - Added a conditional column to map month names to their numeric equivalents (e.g., January → 1, April → 4).

6. **Rename New Column**  
   - Renamed `"Custom"` column to `"MONTH NUMBER"` for clarity.

7. **Change Data Type of Month Number**  
   - Converted `"MONTH NUMBER"` column to whole number type.

8. **Remove Original Month Column**  
   - Dropped the original `"MONTH"` column after extracting numeric month values.

9. **Format Text Columns**  
   - Applied the `Text.Proper` function to categorical text columns (e.g., brand, product type) to standardize formatting.

10. **Final Column Renaming**  
   - Renamed columns to clean, user-friendly names (e.g., `"ITEM ID"` → `"Item Id"`, `"CATEGORY"` → `"Category"`).


