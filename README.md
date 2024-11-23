# Sale Overview Analysis

### Dashboard Link : https://app.powerbi.com/groups/me/reports/b210b468-6f33-4916-a48a-82acb4c443b2/c9ba345b96b0c5274522?experience=power-bi

## Problem Statement

Blinkit, a leading online grocery delivery platform, aims to enhance its operational efficiency and customer satisfaction by leveraging data insights. Despite its rapid growth, the company faces challenges in monitoring and optimizing key performance areas, such as sales, customer ratings, location-specific performance, inventory management, and app usage. The lack of a centralized dashboard limits the ability to make informed, data-driven decisions.

### Steps followed 

You've provided a Power BI file. Here's a step-by-step guide to create a dashboard in Power BI using the uploaded file:

### Step 1: Open the File
1. Launch Power BI Desktop.
2. Open the file you uploaded by navigating to File > Open Report and selecting the `.pbix` file.

### Step 2: Understand the Data
1. In the Fields pane, explore the data tables and columns.
2. Use the Data View to inspect the contents of your tables and understand the available data.

### Step 3: Clean and Transform Data (if required)
1. Go to the Power Query Editor by selecting Transform Data on the Home ribbon.
2. Check for missing values, duplicates, or inconsistencies in your data.
3. Apply necessary transformations like renaming columns, splitting data, or creating calculated columns.

### Step 4: Define Key Metrics and Insights
Identify the key metrics or KPIs you want to display in the dashboard. Examples might include:
- Sales or revenue figures
- Customer acquisition rates
- Inventory levels
- Order fulfillment rates

### Step 5: Create Relationships
1. In the Model View, check if all the tables are correctly related.
2. Create or edit relationships as needed, ensuring they align with your analysis goals.

### Step 6: Build Visualizations
1. Drag and Drop fields into the Report Canvas.
2. Choose appropriate visualizations for your data:
   - Bar/Column Charts for comparisons.

        ![items type](https://github.com/user-attachments/assets/5555814c-d1d0-444a-b438-7c1f56f16e14)

   - Line Charts for trends.

      ![linechart](https://github.com/user-attachments/assets/53cc82d2-4eb0-405a-ac36-99e579d1f446)

   - Pie Charts for proportions.

       ![pie chart](https://github.com/user-attachments/assets/0f7f7836-5341-4b58-8f54-5ad9bdd7c1c8)

   - Tables/Matrixes for detailed data.

     ![outlettype](https://github.com/user-attachments/assets/ecb4d401-ab38-493f-af4f-70c53097519b)

    5.KPI (Key Performance Indicator) is used to represent measurable values

    ![kpi](https://github.com/user-attachments/assets/c5aa27f7-c86d-4ac6-8cf1-a4dc86f27a0e) 


### Step 7: Format Your Visuals
1. Customize colors, labels, and titles for clarity.
2. Add tooltips to provide additional context.

### Step 8: Add Slicers and Filters
1. Use Slicers for user interaction, allowing filtering by date, product category, etc.
2. Apply Page-level Filters or Report-level Filters to control what data is shown.

### Step 9: Arrange and Design the Dashboard
1. Align visuals in a logical order for readability.
2. Group similar insights together.
3. Use Power BI themes or customize the background to make the dashboard visually appealing.

### Step 10: Add DAX Measures 
Create custom measures for advanced calculations, like:

     Avg Rating = AVERAGE('BlinkIT Grocery Data'[Rating])

     Avg sales = AVERAGE('BlinkIT Grocery Data'[Sales])

     No of Items = COUNTROWS('BlinkIT Grocery Data')

     Total Sales = SUM('BlinkIT Grocery Data'[Sales])


     Metrics = {
      ("Total Sales", NAMEOF('BlinkIT Grocery Data'[Total Sales]), 0),
      ("Avg sales", NAMEOF('BlinkIT Grocery Data'[Avg sales]), 1),
      ("No of Items", NAMEOF('BlinkIT Grocery Data'[No of Items]), 2),
      ("Avg Rating", NAMEOF('BlinkIT Grocery Data'[Avg Rating]), 3)
       }


### Step 11: Publish and Share
 Publish the dashboard to the Power BI Service using Home > Publish.

![report](https://github.com/user-attachments/assets/cb5abd6c-9249-4f2d-9c8e-087c53c55b2c)
