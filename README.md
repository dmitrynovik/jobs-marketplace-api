# Problem Statement

We want to build a marketplace outsorcing Jobs to subcontractors backed by an HTTP API.

1. We have Customers with the following mandatory attributes:
    * First Name
    * Last Name
    * ID

2. We have Contractors with the following mandatory attributes:
    * Name (of the business)
    * ID
    * Rating

3. We have Jobs with
    * ID (generated)
    * Start Date
    * Due Date
    * Budget
    * Description
    * Match Strategy
        * Highest rating
        * Lowest price

4. A Customer can create a Job

5. A Contractor can search Jobs and create a JobOffer for a job with `price`

6. 24 Hours before the job Start Date a Job is matched with JobOffers based on the Match Strategy, which creates a Contract.

Create a 2-tier application in C# having a RESTFul API and a persistence layer.
    * CRUD API for Customers
    * The Search API for Customers by its attributes such as ID or Last Name which should be efficient and secure.
    * CRUD API for Contractors
    * The Search API for Contractors by its attributes such as ID or Name which should be efficient and secure.
    * CRUD API for Jobs
    * CRUD API for JobOffers
    * A background job creating contracts
    * The persistence layer can use a data store of your choice (example: PostgreSQL on Docker, SQLite, or just files on disk). 

## What we will be looking at
    * OOP & Solid Principles
    * Input validation.
    * Efficent Data structures (if any).
    * Design patterns.
    * Unit testing.
    * README.md on how to run your solution.
    * Bonus for caching of the Least Recently Using accounts so that the application can scale.


