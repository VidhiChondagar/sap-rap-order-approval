# SAP RAP Order Approval Application

An end-to-end SAP RAP-based Order Approval application built using
ABAP RESTful Application Programming Model (RAP), CDS View Entities,
Fiori Elements, validations, determinations, actions, and mock API
integration.

## 📌 Project Overview

This application provides a Fiori Elements-based interface for managing
Sales Order approval and validation.

The application allows users to:

- Create Order Approval records
- Validate Sales Order items
- Approve or Reject Sales Orders
- Convert Sales Order currency
- Retrieve shipping information
- Display validation, approval, currency, and shipping information

## 🏗️ Architecture

The project follows a layered RAP architecture:

Database Table
↓
Interface CDS View
↓
Projection CDS View
↓
RAP Behavior Definition
↓
Behavior Implementation
↓
Service Definition
↓
Fiori Elements Application

## 🛠️ Technologies Used

- SAP S/4HANA
- ABAP
- ABAP RESTful Application Programming Model (RAP)
- CDS View Entities
- Managed RAP Business Object
- Fiori Elements
- OData
- ABAP Classes
- RAP Actions
- RAP Determinations
- RAP Validations
- Mock API Integration

## ⚙️ Main Features

### Sales Order Validation

The application validates Sales Order items and checks:

- Whether Sales Order items exist
- Material availability in the item
- Valid order quantity

### Approval

Users can approve a Sales Order after successful validation.

### Rejection

Users can reject an Order Approval record.

### Currency Conversion

The application retrieves Sales Order currency information and
performs currency conversion through a mock Currency API class.

### Shipping Information

The application retrieves shipping information through a mock Shipping
API class.

The shipping response provides:

- Shipping Status
- Delivery Days

## 🔄 Application Flow

1. User creates an Order Approval record.
2. Sales Order is entered.
3. Initial approval and validation statuses are determined.
4. Sales Order items are validated.
5. User can approve or reject the order.
6. Currency conversion can be triggered.
7. Shipping information can be retrieved.
8. Results are displayed in the Fiori Elements application.

## 📂 Project Structure

```text
src/
├── CDS/
├── Behavior/
├── Classes/
└── Metadata/

screenshots/
demo/
