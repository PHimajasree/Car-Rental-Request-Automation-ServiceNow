# Car Rental Request Automation in ServiceNow Using Service Catalog and Workflows

## Project Overview

This project automates the car rental request process using ServiceNow Service Catalog and Workflow capabilities. It helps streamline request submission, approval, task assignment, and notification processes while reducing manual intervention.

## Features

- Car Rental Request through Service Catalog
- Transportation Services catalog category
- Request details captured using catalog variables
- Automated approval using Flow Designer
- Conditional processing based on approval status
- Catalog task creation and assignment to Transport Team
- Email notification triggers
- Business Rule for handling car unavailability
- Request and task status tracking
- Update Set migration between ServiceNow instances

## Catalog Variables

- Requestor
- Requested Date
- Pickup Location
- Drop Location
- Duration (hrs)
- Car Type
- Reason1

## Flow

The `Car Rental Req` flow handles the request lifecycle:

Request Submitted → Approval → Approval Validation → Catalog Task → Get Catalog Variables → Email Notification

## Business Rule

**Create Incident if Car Unavailable**

The Business Rule is configured on the Requested Item table and creates an Incident when the required condition is met.

## Update Set

The ServiceNow Update Set XML containing the project configuration is included in this repository.

**Update Set:** `Car Rental Request Setup`

## Technologies Used

- ServiceNow
- Service Catalog
- Flow Designer
- Business Rules
- Update Sets

## Project Status

Completed
