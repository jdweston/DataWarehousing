# DataWarehousing
This project demonstrates designing and creating a staging data warehouse using PgAdmin and PostgreSQL that will hold download-only retail sales. Once created, I have stored data into their corresponding tables and queried the data to uncover sales details about the products.

The project is viewable via code snippets and screenshots in the images folder, and I will explain each image and what is going on below.

To start the project, I was given a sample of data to base my star schema off of (shown in "sample_data.jpg"). I was tasked with creating the warehouse in a way that allowed the company to create reports on a yearly, monthly, quarterly and daily basis based on category and/or country. 

In a database titled 'softcart', I created various Dimension tables (as shown in the images/tables folder) in order to get the full extent of information needed. Once created, I linked the tables with the Fact table for easier querying between them. The relationship can be seen in the ERD of the image "softcartRelationships.jpg".

My next task was loading the tables with data, that can be found in the data folder, and creating complex queries to view sales data from different perspectives using rollup, cube, and grouping sets queries (shown in images with their respective names).

Finally I created a Materialized View of the data to show the total sales of each country in alphabetical order, found in "mqt.jpg".