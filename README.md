# Build-an-AI-Enabled-FinTech-B2B-Invoice-Management-Application

In this project, I built a web application to help the
people working in the Accounts Receivable departments in their day-to-day
activities.I build a web application where the users in the Account
Receivable department can :
● View the invoice data from various buyers.
● See various fields/attributes of the invoice(s) from a particular buye
● Perform Data Pre-processing on the invoice data.
● Get account-level analytics to easily visualize and interpret data- EDA and
Feature Engineering.
● Get a prediction of when the invoice is going to get paid.


## Business Overview

### Introduction to B2B Operations:
The B2B world operates differently from the B2C or C2C world. Businesses
work with other businesses on credit. When a buyer business orders goods
from the seller business, the seller business issues an invoice for the same.
This invoice for the goods contains various information like the details of the
goods purchased and when it should be paid. This is known in accounting
terminology as “Accounts Receivable”.

“Accounts Receivable represents money owed by entities to the firm on the
sale of products or services on credit. In most business entities, accounts
receivable is typically executed by generating an invoice and either mailing
or electronically delivering it to the customer, who, in turn, must pay it within
an established timeframe, called credit terms or payment terms.”

Seller business interacts with various businesses and sells goods to all of them
at various times. Hence, the seller business needs to keep track of the total
amount it owes from all the buyers. This involves keeping track of all invoices
from all the buyers. Each invoice will have various important fields like
payment due date, invoice date, invoice amount, baseline date etc.
The buyer business needs to clear its amount due before the due date. However,
in real-world scenarios, the invoices are not always cleared ie. paid in full
amount by the due date. The date on which a customer clears the payment for
an invoice is called the payment date.


### Account receivables Department:

In the ideal world, the buyer business should pay back within the
stipulated time (ie the Payment Term). However, in the real world, the
buyer business seldom pays within their established time frame, and this
is where the Account Receivables Department comes into the picture.
2. Every business consists of a dedicated Account receivables Department to
collect and track payment of invoices.
3. It consists of an Account receivables team that is responsible for:
● Collecting payments from customers for their past due to invoices.
● Sending reminders and follow-ups to the customers for payments to be
made.
● Looking after the entire process of getting the cash inflo
● Help the company get paid for the services and products supplied.


## Problem Statement for ML:

As a winter internship project, you will be building a web application to help the
people working in the Accounts Receivable departments in their day-to-day
activities. You need to build a web application where the users in the Account
Receivable department can :
● View the invoice data from various buyers.
● See various fields/attributes of the invoice(s) from a particular buye
● Perform Data Pre-processing on the invoice data.
● Get account-level analytics to easily visualize and interpret data- EDA and
Feature Engineering.
● Get a prediction of when the invoice is going to get paid.

## Problem Statement for Web Application Development:

The objective of the Web Application Development internship project is:
● To build a Full-stack Invoice Management Application using ReactJs,
JDBC, Java, Servlets.
● Build a responsive Receivables Dashboard.
● Visualize Data in the form of grids.
● Visualize Data in the form of graphs.
● Perform Searching operations on the invoices.
● Add & Edit data in the editable fields of the gri
● Delete data of selected rows in predefined templates.

## React Web App

The mandatory features are compulsory tasks and the optional features are for
extra credit points, which will give you an added advantage.

### Mandatory Features

1. UI Creation
2. Grid Creation
3. Grid Data Loading
4. Crud Operation
a) Add
b) Edit
c) Delete
5. Pagination
6. Advanced Search

### Optional Features

1. Predict Button activation
with Grid Data
2. Shortcut search button on
Grid for Customer Id
3. Sorting columns
4. View - Analytics

## HIGH-LEVEL REQUIREMENTS OF APPLICATION

Specifically, below are the major aspects of the application that needs to be develope
The details for each of the below are provided in the functional overview section.

### 1) Data Loading in DB:
● You will be provided with an invoices dataset which you need to parse,
process, and load in the provided database schemas.

### 2) UI Representation of the data:
● Build a responsive UI that can display the invoice data loaded from the
database.
● The UI should support searching and pagination
● The UI should support editing of some editable fields, adding a new r
to the grid, deleting rows from the grid and advance search.

### 3) AI Support in the application:
● Add support for predicting the payment date for one or more invoice(s).
● UI should have a button to trigger the prediction of the payment date.
● The payment date needs to be persisted across sessions in the UI.

## FUNCTIONAL OVERVIEW

### (1) Data Loading in the Database
Below is the sample CSV file screenshot 

![snip1](https://github.com/user-attachments/assets/2710925d-b945-4314-b4ce-dd79d88607dc)

All the Columns of the CSV file need to be loaded into the DB

![snip2](https://github.com/user-attachments/assets/68f4877f-e671-43d6-89ad-6b3ec42b5ad8)

### (2) UI Representation of the Data:

The UI consists of a single screen :

![snip3](https://github.com/user-attachments/assets/2cb8f3f3-1828-4bde-807d-a3e1c53317a1)

#### Receivables Dashboard Page
It consists of 2 sections:

##### Header:
a. First Section is the header which comprises the ABC Product logo on the
left, the Highradius Logo in the middle
b. The second section consists of Predict, Advance Search, Analytics View
Add, Delete & Edit, and Search bar.

##### Add button:
● It is used for adding new field values to the gri
● The Add button will be in the enabled state if no row is selected.
● Whenever one or more rows are selected, the Add button will still remain activated.
● After clicking on the Add button, a pop-up window will appear with all the fields for
which values need to be added along with a Cancel and an Add button.
● The user should be able to type in the values, except for the date of the invoice for
which there should be a calendar view from where the user is able to select the required
date, month, and year.
● The user should fill in all the required fields before adding. If the user tries to click on
add before all mandatory fields are filled, the user will not be able to add.

![Capture](https://github.com/user-attachments/assets/1c492c80-9799-46ca-8135-9e662a8ed920)

Full-Screen View

![snip4](https://github.com/user-attachments/assets/db9b0049-24b7-4c7a-ae51-2861980107b3)

##### Edit button:
● It is used for editing the editable field values in the gri
● Edit button should be disabled at first and should enable only one checkbox 
selected
● A user should be able to select a row and then click on the Edit button.
● The fields which can be edited are the Invoice Currency and Custom
Payment Terms field
Without selecting any row, the Edit button should remain disabled.
● On clicking the Edit button, a popup should open up with the column header
name and existing value. The user should be able to edit the existing value.
● The popup should have a Edit, Cancel as shown in the UI below.

![snip5](https://github.com/user-attachments/assets/743b4c58-e620-49d0-96bb-81d579cde968)


Full Screen View 

![snip6](https://github.com/user-attachments/assets/157910e2-a079-41a3-a130-94c02448dbb7)

##### Delete Button :
● Clicking on the delete button will allow the user to delete records from the grid.
● When the user selects one or more rows, the delete button gets enabled.
● A pop-up should be displayed on clicking delete to confirm that the user wants to delete
the selected records permanently.
● Once the user clicks on the delete button, the row(s) should be removed from the grid in
the UI and should remain persistent.


![snip7](https://github.com/user-attachments/assets/cf4f0a6e-cde6-4ace-a684-c2ce613f8711)

Full Screen View

![snip8](https://github.com/user-attachments/assets/7a3efb9b-0f67-4bc7-b57c-53fb513d121b)

##### Predict button:

● Users should be able to predict the payment date of selected Invoices with the
help of the Predict button.
● Clicking on this button will populate the Predicted Payment Date column on the
UI with the predicted dates.
● When the user selects one or more Invoices and clicks on the Predict button, the
Predicted Payment Date column should get populated only for those invoices.
● The button should get activated only upon selecting any of the Invoice(s).
● If no Invoice is selected, the button should be in a disabled state.


![snip9](https://github.com/user-attachments/assets/83f02b38-2f17-488f-a6d4-5a8a1403458c)

##### Advanced Search button:

The UI consists of the Advanced Search button.
Clicking on this button will help the user to perform an advanced search on the data
based on the following four field
1. Document Id-(doc_id)
2. Customer No-(cust_number)
3. Invoice No-(invoice_id)
4. Business Year- (buisness_year)

![snip11](https://github.com/user-attachments/assets/65138d73-223c-44e1-9b73-2d8cccd5adbf)

Full Screen View

![snip12](https://github.com/user-attachments/assets/9e04f97f-4de6-4744-bfee-096c3df88f89)

##### Analytics View: (Optional Task)

To get insights from the existing data based on users inputs. The existing parameters
would act as key points or outliers for the synthesis of data.
So the analytics view will be a button in UI which responds to a new window on click
event

![snip13](https://github.com/user-attachments/assets/0e37427c-22bf-4e53-b06a-fb26e2775ba0)

The new window contains of parameters:
Currency (Multiselect)
Due Date
Baseline Create Date
Clear Date
The user will have a privilege to go for single parameter or multi parameter based on
their choices and preferences.
On submitting the parameters the web application will open the dialog window which
will provide the user with an illustration of a bar graph and pie chart which will be
formed based on the parameterized data that the user had selected.
The bar graph will be showing data for the total open amount and number of customers
for all Business


![snip14](https://github.com/user-attachments/assets/cd9a00e8-cd3f-4bfd-929f-5e35f5ba2601)

Pie Chart for Currencies :The Pie chart will be containing the selected currencies.


![snip15](https://github.com/user-attachments/assets/256f7692-212c-4b1d-ab8f-92bc72821f3d)


##### Searchable fields behavior:

a.Business Year- Text Field
b.Customer Id-Text Field
c.Invoice No - Text Field
d.Document Id - Text Field
e.Customer Id - Equal Search
Users should be able to search for a customer by typing text in the Customer id integer
field. Search is not case-sensitive.

![snip16](https://github.com/user-attachments/assets/8434c71e-a224-4442-a830-da846ecf17d3)


##### Grid Panel Section

The Seventh Section is the Grid Header section, consisting of all the different column
name headers and a Select All and Deselect All functionality.
Following are the columns to be displayed in the UI:
1. sl_no
2. business_code
3. cust_number
4. clear_date
5. buisness_year
6. doc_id
7. posting_date
8. document_create_date
9. due_in_date
10.invoice_currency
11.document type
12.posting_id
13.total_open_amount
14.baseline_create_date
15.cust_payment_terms
16.invoice_id

![snip17](https://github.com/user-attachments/assets/d3dc3236-6214-4466-86f3-cc8a1ea54dba)

##### The Grid panel section will be divided into 3 portions:

● The header of the grid will have a Predict button on the top left corner followed
by an Advance Search Button,an Analytics view, an Add Button, an Edit Button,
a Delete Button, and a Search Bar.
● The name of the grid that is Invoice List will be mentioned in the top left corner of
the grid.
● The second portion is the table with customer invoice data as rows and the
following columns:

The list of all the columns to be represented on the UI are as follows:
1. sl_no
2. business_code
3. cust_number
4. clear_date
5. buisness_year
6. doc_id
7. posting_date
8. document_create_date
9. due_in_date
10. invoice_currency
11. document type
12. posting_id
13. total_open_amount
14. baseline_create_date
15. cust_payment_terms
16. invoice_id


The Grid consists of the Grid Rows that contains the required data that is loaded from
the CSV File. On a single page, only 10 invoices’ data is displayed. Users can select
single or multiple rows

![snip18](https://github.com/user-attachments/assets/5080b6a8-9f97-4fca-bc32-d86ad53a2a1b)

##### Sorting & Searching

1. Sorting:
Sorting should be performed on all the columns:
2. Clicking on the column headers should sort the values of the whole grid
a. First click - Ascending
b. Second click - Descending
Column headers should have a double arrow symbol near the column name to
indicate they can be sorted.

##### Horizontal Scroll Bar

The Horizontal Scroll Bar which can be used to scroll across the screen to access the data in various columns.

##### Footer

The Grid consists of the Footer which will have the following three parts:
● 'Viewing <starting count> - < end count> of <total count>' text on left. It shows
invoices currently active.
Example1: Viewing 1-10 of 500 means that the user is seeing 1-10 Invoices
present on the page out of the total number of invoices which is 500.
● Pagination arrows with text ' <present page number> of <total page number> ' in
center. Clicking on the back arrow takes the user to the previous page. Clicking on the
next arrow takes the user to the next page. Back arrow should be disabled when the
user is on the first page and the next arrow should remain disabled if the user is on
the last page.
Example2: 2 of 50 means that the user is currently on 2ndd page and seeing
invoices 11-20 out of the total 500 invoices.
● 'Copyright 2022 Highradius.All Rights Reserved.' in the middle.

##### AI support for the prediction of payment date

1. As part of this project, you need to predict the Payment Date of each invoice.
2. In order to achieve this, there should be a button named “Predict” present on
the UI besides the “Advance Search” button.
3. Users can select one or more invoices and click on the “Predict” button to
predict the payment dates of those selected invoices.
4. Once the button is clicked, the Predicted Payment Date column should get
populated with the predicted dates derived from the ML model.
5. The “Predict” button should remain disabled if no invoices are selected.

##### Glossary

1. Invoice - A document that is issued by a seller to a buyer when some goods are
purchased. The fields which can be part of the invoice are defined b
2. Advanced Search - A pop-up window, which depicts the illustration that
enables the user to search with single or multiple parameter values from the
grid.
3. Predict - The predict button is used as a tool to predict the Payment Date of
each invoice.































































































































































































































































































