IT Ticket Automation Workflow
Overview

This project automates the processing of internal IT support tickets for a university using n8n Desktop. The workflow handles tickets end-to-end, including validation, routing, SLA calculation, and reporting.

The system reduces manual errors, avoids duplicate tickets, and provides a team summary of workload.

Features
Features

Ticket Validation: Checks email format and priority (High, Medium, Low).

Rejected Tickets: Invalid tickets are separated for review.

Normalization: Cleans text fields (Name, Email, IssueType, Description).

Ticket ID Generation: Automatically assigns a unique ID to each ticket.

Routing: Assigns tickets to the correct team based on IssueType:

IssueType	Team
wifi	Network
login	IT Support
software	Applications
hardware	Infrastructure
other	General
SLA Calculation: Calculates deadlines based on priority: High = 4h, Medium = 24h, Low = 72h.

Team Summary: Counts tickets per team to provide an overview of workload.


nsert your n8n Desktop workflow screenshot here.

The workflow includes:

Tickets Input (sample tickets in Function Node)

Validation (email and priority)

IF Node to separate rejected tickets

Normalization

Timestamp Fixing

Ticket ID Generation

Routing to teams

SLA Calculation

Processed Tickets CSV

Team Summary CSV

n8n Desktop – main workflow automation tool

Function Nodes – for processing, calculations, routing, and SLA

IF Nodes – for validation and branching

CSV Nodes – for saving processed and rejected tickets
