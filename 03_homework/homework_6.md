# Homework 6: Reflecton

- Due on Saturday, May 25 at 11:59pm
- Weight: 8% of total grade

<br>

**Write**: Reflect on your previous work and how you would adjust to include ethics and inequity components. Total length should be a few paragraphs, no more than one page.

For the past couple of weeks, I have been using SQL data to retrieve, manipulate and update data for a hypothetical farmers market. There are several data ethics considerations that can be learnt from these activities that I will be applying in my role going forward. First and foremost is ensuring that individuals and enterprises are aware and sign-off that you are allowed to capture their data. There should also be strong privacy policies adhered to, such as an understanding of who has access to the data, where the data is to be stored and what the data can be used for. The database should also be architected to ensure that the bare-minimum data is captured to achieve the insights required and that the database architecture does not combine information (and tables) that could be used to deanonymize confidential information that could jeopardize an individual or enterprise’s identity, privacy, security or proprietary information.

The ethics course on Thursday also had me thinking about how this data was collected and entered into a database. In a lot of cases, manual data entry is required to convert analog data (eg hand written forms) into digital data for a database. It is important that the people who are providing their labor to complete these tasks are paid fairly and treated fairly, with their health being a priority. Finally, the ethics course reminded me to think about different biases that could arise when building the database architecture and performing data entry.

A couple of examples from the hypothetical farmers market that got me thinking include:
- Were the customers and vendors aware and signed off that this data was being collected and visible to so many people? How should this database be restricted to its many users?
- In one of the earlier homework exercises there was a Farmer Market Appreciated Committee that gave out bumper stickers to customer who were high spenders. This had an element of stalking and neglection of other customers who may share an appreciation/patronage for attending farmers markets but have different income levels. Better inclusion here could actually be financially rewarding as bumper stickers on cars with customers who spend less could promote the farmer market in different areas of the city, bringing in more and diverse groups to the market.
- The inclusion of customer names and respective zip codes was not relevant for a high majority of the SQL tasks and questions whether this data should have been captured in the database in the first place
- The CROSSJOIN task in homework five creates a table that gives away proprietary and sensitive information about vendors and customers. Additional security and access policies need to be in place for these aggregated tables.
