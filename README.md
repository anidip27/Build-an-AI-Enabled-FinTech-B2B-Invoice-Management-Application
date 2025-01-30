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

#####Add button:
● It is used for adding new field values to the gri
● The Add button will be in the enabled state if no row is selected.
● Whenever one or more rows are selected, the Add button will still remain activated.
● After clicking on the Add button, a pop-up window will appear with all the fields for
which values need to be added along with a Cancel and an Add button.
● The user should be able to type in the values, except for the date of the invoice for
which there should be a calendar view from where the user is able to select the required
date, month, and year.
● The user should fill in all the required fields before adding. If the user tries to click on
add before all mandatory fields are filled, the user will not be able to add


