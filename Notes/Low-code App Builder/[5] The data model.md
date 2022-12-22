# The data model

- [The data model](#the-data-model)
    - [1. Data modelling](#1-data-modelling)
        - [1.1. Data Storage](#11-data-storage)
        - [1.2. Data modeling best practices](#12-data-modeling-best-practices)
            - [1.2.1. Addition of data through a UI view](#121-addition-of-data-through-a-ui-view)
    - [2. Data records](#2-data-records)
        - [2.1. Data records and data objects](#21-data-records-and-data-objects)
        - [2.2. Local data storage](#22-local-data-storage)
        - [2.3. External data sources](#23-external-data-sources)
    - [3. Data pages and the Visual Data Model](#3-data-pages-and-the-visual-data-model)
        - [3.1. Default data pages for data objects](#31-default-data-pages-for-data-objects)
        - [3.2. Simulated data pages](#32-simulated-data-pages)
    - [4. Integration designer](#4-integration-designer)
        - [4.1. Integration Designer landing page](#41-integration-designer-landing-page)
        - [4.2. Integration Map](#42-integration-map)

## 1. Data modelling

**Data modeling** is the process by which data elements arrive into your application in a format that makes sense for your business and are then processed, reported on, and stored.

**Data model** defines the types and structures of data in your application and standardizes how data elements relate to one another.

Components to model data:

1. **Fields** - Properties that store and format data in your application
2. **Data objects** - Categories of data that have fields, field mappings, and connection to data sources.

### 1.1. Data Storage

It is best practice to create a data class with the same name as the case type to store data that is not found n existing data objects instead of storing it in on the work object. such as a case.

### 1.2. Data modeling best practices

Verify the data model with a Lead System Architect before creating data objects or properties.

#### 1.2.1. Addition of data through a UI view

- Create the data model by using the **Data Explorer** first, keeping reuse and inheritance in mind.
- Use the **Configure a view** to add new fields as needed throughout the application's update life cycle.

## 2. Data records

- Data records define permissible values for data fields. Limiting the input values to valid options reduces errors and allows for automation.
- can be stored outside the case
- can be reused and referenced
- by default, data records are displayed as a selectable drop-down list

### 2.1. Data records and data objects

**Data objects** (columns/fields)

- represents key business entities
- contain all the fields necessary to describe an object
- a change on data object fields represents a change in the business process

**Data records** (rows/records)
- a change on data record values does not need an asoociated change in the business process to support the change

### 2.2. Local data storage

lets you store data records for a data object without creating or maintaining database tables.

### 2.3. External data sources

You can configure a data object to retrieve data from an external data source, such as a database or a web service.

## 3. Data pages and the Visual Data Model

**Data pages**

- Shows how your application uses data and defines the data associated with a data object.
- Data pages provide links between data records and your application.
- identifies how to connect the system of record and what fields to map in the data object.
- allows an application to populate data reference with source data

**Visual Data Model**
- a diagram that shows these links by providing visibility into the applications's data model and how the entities are related.
- can update, add, and delete fields

### 3.1. Default data pages for data objects

Three default data pages for data objects configured to a system of record:

1. Single - returns a single record
2. List - returns all data records of a data type
3. Savable - allows a case to save a single record to the system of record

### 3.2. Simulated data pages

You can use a simulated data source during application development and testing but you must configure the connected to a data source before the data pages are ready for production.

## 4. Integration designer

### 4.1. Integration Designer landing page

provides a single location in App Studio for viewing all the data objects, data pages, object dependencies, and external systems in an application.

### 4.2. Integration Map

A diagram of the data objects, cases, and systems of record in the application and where they are sourced.
