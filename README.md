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































