# Project Management Software

This is a project management software used by companies to manage their software development processes for every project they take on. Companies can add projects, multiple features under each project, and multiple boards/issues under specific features. The software tracks the status of the processes from start to end.

Customers who subscribe to a feature are notified by email throughout the entire process.

## Accounts

All the users in the system are stored in the accounts table; customers, admin, project manager, and software developers. All accounts belong to a specific company.

## Employee

Stores information about the employees who manage everything on the company account.

The Employee entity is a child entity of the Accounts entity in the inheritance structure.

## Companies

Stores the company information like title description and anything specific to the company. It has several/many accounts that manage its tickets.

## Project

A high-level overview of what the company is working on, it's a full project at this stage. For example, the project management we are working on here is a ride-booking app, and so on.

A company can have multiple projects, mostly a software company or a multi-project company like Meta.

## Features

A high-level overview of what needs to be worked on under a specific project. For example authentication, messaging, etc.

## Boards

Represents a breakdown of what has to be worked on under a specific feature, for example, if a login.

## Customers

Customers subscribe to a board and they are notified every time the board moves from one stage to another, in this case, from issue, working, released. 

The Customer entity is a child entity to the Accounts entity in the inheritance structure.

## Emails

Stores the email sent to the customers.
