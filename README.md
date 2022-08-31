Amazon Webpage Query

This sample is a basic Web query for Amazon’s Top 30 OTC items. It automatically queries the webpage organizes the query in a readable list that contains the item rating and price. It can be extended to Top 100 if necessary. Vlookups are used but the main function to organize the list is the offset function. Offset is used to return the cell details in a list where the formula references the next 5th row down. (Currently had to adjust the formula in item 7 since data was missing in the query solely for this item).

Formulas:

• =Query!A17

• =OFFSET(Query!A$17,(ROW()*0)+$B6,0)

Query Connection String:

• https://www.amazon.com/Best-Sellers-Health-Personal-Care-OTC-Medications-Treatments/zgbs/hpc/10079990011
