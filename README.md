# developer-challenge-data-modeling
Simple data modeling challenge for backend interview candidates.

## Installation
Just clone the repo.  You will need sqlite3.  There's a sqlite3 database in the `/db/` folder that you can use to write queries against.  Use a *.sql file to house any queries you wish to persist and run.  You can execute a sql file against the sqlite database using a similar pattern:

```
sqlite3 db/customer_admin < sql_query.sql
```

## The Exercise
1. Hypothetical scenario, the company wants to create a database for a simple ordering application; how would we create tables for the following things?  Ideally we would like to prevent admins from deleting products or customers if there are associated orders.  All fields are required unless stated otherwise:
    - Products
        - Name
        - Product Type
        - Cost
    - Orders
        - Product ID
        - Customer ID
        - Amount
        - Order Date
    - Customers
        - Name
        - Contact First Name
        - Contact Last Name
        - Contact Email
        - Contact Phone (not required)
        - Country
2. Hypothetical scenario, we want to be able to support a basic subscription system with a number of plans; how would we change the database to support that?