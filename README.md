# DataStage-Project-Retail-DataWarehousing


Overview:
This project focuses on building a star-schema data warehousing flow using IBM InfoSphere DataStage for a fictitious national department store. The goal is to create a sales analysis data warehouse with dimensions such as customer, store, and product. The data warehouse should accommodate changing dimension attributes over time while preserving historical information.


Prerequisites:
- IBM InfoSphere DataStage installed and configured.
- Access to the OLTP system as the data source.

## Project Setup
To set up the project, follow the steps below:

1. **Star-schema Design:** Design the star-schema model, including dimension tables (customer, store, product) and the fact table (transactions).
2. **Data Population:** Populate the dimension tables and fact table with sample data. Refer to the attached files for sample data.
3. **Recurring Tasks Setup:** Set up the necessary configurations for recurring tasks.

## ETL Solution
The ETL solution is responsible for loading the data into files or databases based on specific business needs. It involves reading the source data, performing transformations, and loading the transformed data into the data marts. The key requirements and transformations are as follows:

### 1. Building the "RETAIL_DATA_MART"
- Requirement: Create a data mart that displays each transaction for customers based on their type (citizen or foreign), including product information and stock details.
- Transformation: Perform uppercase transformation on the customer name column.
- Output: Generate the "RETAIL_DATA_MART" file.

### 2. Creating the "ACTIVATIONSALES_DATA_MART"
- Requirement: Analyze the "ACTIVATIONSALES_DATA_MART" data mart to address specific business needs.
- Transformations:
   - Display the count of all transactions for each employee in each store.
   - Determine the customer type (citizen or foreign) that generated the maximum profit.
   - Calculate and assign a bonus to profitable customers using the equation: Annual_Incomek$ * SpendingScore * 100.
- Output: Generate insights and results based on the transformations.

