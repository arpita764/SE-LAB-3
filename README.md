# SE-LAB-3
# Self-Service Coffee Kiosk System

## Overview

This repository contains the deliverables for **Lab 3 – Architecture Selection and Justification** for the Self-Service Coffee Kiosk System.

The system is designed as a self-service coffee kiosk that allows customers to select a coffee type and size, make a credit-card payment, and receive a printed receipt. The system also stores and retrieves menu and pricing information.

## Architecture

The selected architecture is **Layered Architecture**, organized into three layers:

### 1. Presentation Layer

Contains the:

* User Interface Component

The User Interface provides the touch-screen interaction through which customers select their coffee type and size.

### 2. Business Layer

Contains:

* Order Manager Component
* Payment Service Component
* Receipt Printer Component

The Order Manager coordinates order processing and communicates with the payment service, receipt printer, and menu database.

### 3. Data Layer

Contains:

* Menu Database Component

The Menu Database stores menu and pricing information required by the system.

## Component Interfaces

The component diagram contains four main interfaces:

| Interface            | Purpose                                                               |
| -------------------- | --------------------------------------------------------------------- |
| Order Interface      | Handles order submission from the User Interface to the Order Manager |
| Payment Interface    | Handles credit-card payment requests                                  |
| Receipt Interface    | Handles receipt data and print requests                               |
| Menu/Price Interface | Handles database queries for menu and pricing information             |

The diagram uses UML **provided interfaces (ball)** and **required interfaces (socket)** to represent the interactions between components.

## Deliverables

### Component Diagram

The component diagram shows:

* Five system components
* Four component interfaces
* Provided and required UML interfaces
* Component interactions and data flow
* Presentation, Business, and Data layers

**File:** `Lab3_Component_Diagram.pdf`

### Architecture Justification

The architecture justification explains:

* The selected Layered Architecture
* Two reasons for selecting the architecture
* A security advantage
* A performance benefit

**File:** `Lab3_Architecture_Justification.pdf`

## Repository Structure

```text
Lab3-Coffee-Kiosk/
│
├── README.md
│
├── Lab3_Component_Diagram.pdf
│
└── Lab3_Architecture_Justification.pdf
```

## Conclusion

The Lab 3 deliverables demonstrate the architecture and component interactions of the Self-Service Coffee Kiosk System using a layered architectural approach. The design separates presentation, business processing, and data storage responsibilities while clearly representing the required component interfaces and data flow.
