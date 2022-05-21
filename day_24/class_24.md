[Dynamic API Server Live Url](https://mujahedyousef.github.io/advanced-js-reading-notes.-/day_24/class_24.html)

# Dynamic API Server

> An Express/Node.js based server designed to be a “model agnostic” REST API server, which can perform CRUD operations on any data model.

## Support all REST/HTTP methods

* GET: Retrieve record(s) from a data source
  * All
  * One (by id)
  * Some (by filtering)
* POST: Create a new record in a data source
* PUT: Update a single full record in a data source
* PATCH: Update part of a single record in a data source
* DELETE: Delete a record in a data source

## Development Process, Milestones

* Phase 1: API Basics
  * Use JSON Server (non-express) to mock the routes for testing purposes
* Phase 2:
  * Basic API
Create CRUD/ReST endpoints for categories and products

  * Separate route modules for each data model type
  * Store user created data in memory (no persistence)
  * Integrates with an online CI framework

* Phase 3: Persistence
  * Replace the in-memory data store with mongo
  * Use Mongo Collections for each data model type
* Phase 4: Dynamic Models
  * Create a single model class that all data models can inherit from to keep the interface simple
  * Use middleware to load models based on param
i.e. Replace app.get('/api/v1/categories') and app.get('/api/v1/products') with app.get('/api/v1/:model')

----

## Authentication Server / Module

> An Express/Node.js based server using a custom “authentication” module that is designed to handle user registration and sign in using Basic, Bearer, or OAuth along with a custom “authorization” module that will grant/deny users access to the server based on their role or permissions level.

### Development Process, Milestones

* Phase 1: Basic Authentication

- Create a basic express server with the following features:

  * Users Model (Mongoose Schema)
  * /signup route that creates a user
  * /signin route that attempts to log a user in
  * BasicAuth middleware that validates the user as a part of the /signin process

* Implement: Modularize and Test a starter server
* Phase 2: Bearer Authentication
  * Re-Authenticate Users
  * Accepts a TOKEN in the Authorization: Bearer header
  * Validates the user
  * Allows or Denies access to the route handler
  * Implement: Debug, Extend Token Security
* Phase 3: Authorization
  * Role Based Authorization System
  * Combines the Bearer Token with User roles to give fine grained access control
  * Implement: Protect API Routes, Write tests
