# Problem Statement

We want to build a marketplace outsorcing Jobs to subcontractors backed by an HTTP API.

1. We have `Customer`s with the following mandatory attributes:
    * First Name
    * Last Name
    * ID

2. We have `Contractor`s with the following mandatory attributes:
    * Name (of the business)
    * ID
    * Rating

3. We have `Job`s with
    * ID (generated)
    * Start Date
    * Due Date
    * Budget
    * Description
    * AcceptedBy

4. A Customer can create a `Job`

5. A Contractor can search `Jobs` and create a `JobOffer` for a job with `price`

6. A Customer can accept a `JobOffer` which creates a `Contract`

# Requirements
Create a 2-tier application in C# having a RESTFul API and a persistence layer:
* The Search API for Customers by its attributes such as ID or a part of Last Name which should be efficient and secure.
  * Example: `GET /customers/smi` may return `[{ Name: "John", LastName: "Smith"} ]`
* The Search API for Contractors by its attributes such as ID or Name which should be efficient and secure.
* CRUD API for Jobs with appropriate validation
* CRUD API for JobOffers with appropriate validation
* The persistence layer can use a data store of your choice (example: PostgreSQL on Docker, SQLite, files on disk, or just memory with a right abstraction).
* IMPORTANT: The system needs to scale. Say, we aim to have 100 000 businesses and 10 million customers.
 
# Hints:
* You may seed some data such as Customers and Contractors in the system.

## What we will be looking at
* OOP & Solid Principles
* Input validation.
* Efficent Data structures (if applicable).
* Design patterns.
* Unit testing.
* README.md on how to run your solution.
* Bonus for caching of the Least Recently Using accounts so that the application can scale.


