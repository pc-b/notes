---
id: d7d3sicgwjatqx4ma8noypc
title: Relationalmodels
desc: ''
updated: 1694611696130
created: 1694611557234
---
# Data Models:

-   A data model is **abstract** (generalized) representation that organizes elements of data and **standardizes** how they relate to one another and to the properties of real-world entities

### Example - database of books:

-   Author

-   Title

-   Publisher

-   Pub date

-   Price

-   ISBN

*How do we describe this data?*

# Relational Data Models:

-   Relational data models are data models that represent the database as a collection of relations

-   A table of values

-   Every row in the table represents a collection of related data values

## Terminology

-   A **relation** is a table with columns and rows

    -   A relation corresponds to an entity set, or a collection of entities

-   An **attribute** is a named column of a relation. Also corresponds to a characteristic of an entity. Also called fields

-   A **tuple** is a row of a relation

-   **Degree** is the number of attributes of a relation

-   **Cardinality** is the number of tuples in a relation

-   **Domain** is the set of allowable values for one or more attributes

# Elements of Data Models:

-   Instance

    -   The actual data

-   Database schema

    -   A database schema represents the logical configuration of all or part of a relational database

    -   In logic design phase

-   Query language

    -   How to create database, retrieve and manipulate data

    -   DDL

    -   DML
# Relational Data Model - cont:

-   Data is a collection of relations / tables

    -   Relation is a set of tuples

    -   Each tuple appears 0 or 1 times in table

    -   Order of rows unspecified

-   Rows = tuples = records

-   Columns = attributes = fields

-   Degree of relation = \# attribute

-   Each attribute has a type

    -   Always becomes data in computer

    -   Has data type

    -   Ex.

    -   Strings:

        -   CHAR(20)

        -   VARCHAR(20)

        -   TEXT

    -   Numbers:

        -   INT

        -   SMALLINT

        -   FLOAT

        -   MONEY

        -   DATETIME

-   Attribute is statically and strictly enforced, occurs in database creation
# Primary Key:

-   Attribute that uniquely identifies a record
# Foreign Key

-   A set of attribute in a table that refers to the primary key of another table

    -   Company(cname, country, nonemployees\', for_profit)

    -   Country(name, population)

| Cname   | Country | No_employees | For_profit |
|---------|---------|--------------|------------|
| Canon   | Japan   | 50000        | Y          |
| Hitachi | Japan   | 30000        | Y          |

 

| Name  | Population |
|-------|------------|
| USA   | 320M       |
| Japan | 127M       |
# Multi-attribute key

-   A composite key is a key that consists of two or more attributes that together uniquely identify an entity occurrence

-   Not recommended in this course
# Summary - keys:

-   Primary key

    -   Attribute that uniquely identify tuple

    -   Usually database designer defines it

    -   Relation can have many keys, but only one is primary key

-   Foreign key

    -   Attributes that is a primary key ofa record in other relation

    -   Foreign in foreign key is related to certain tables

    -   Does not require uniqueness
# Notes on tables

-   Tables are NOT ordered

-   Records in table are organized by primary keys

-   Tables are flat, no nested attributes