# Inventory Management System.

The Inventory Management System is a desktop application built to manage inventory for a small manufacturing organization. Users can create, view, and manage parts and products.

![App UI](https://imgur.com/mwhp5cx.jpg)

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Setup](#setup)
- [User Interface](#user-interface)
- [Application Functionality](#application-functionality)
- [Exception Handling](#exception-handling)
- [Contributing](#contributing)
- [License](#license)

## Overview

The Inventory Management System provides a platform to manage inventory efficiently. Users can add, modify, delete, and search for parts and products.

## Features

- **User Interface:** A graphical user interface (GUI) for managing parts and products.
- **Part Management:** Add, modify, and delete parts.
- **Product Management:** Add, modify, and delete products.
- **Search Functionality:** Search for parts and products.
- **Exception Handling:** Ensures application stability and improves user experience.

## Tech Stack

- **Language:** C#
- **IDE:** Visual Studio
- **Framework:** .NET

## Setup

1. Clone this repository.
2. Open the project in Visual Studio.
3. Build and run the application.

## User Interface

The application includes the following forms:

### Main Form

- **Controls:**
  - Buttons for “Add,” “Modify,” “Delete,” “Search” for parts and products, and “Exit”
  - Lists for parts and products
  - Text boxes for searching for parts and products
  - Title labels for parts, products, and the application title

### Add Part Form

- **Controls:**
  - Radio buttons for “In-House” and “Outsourced” parts
  - Buttons for “Save” and “Cancel”
  - Text boxes for ID, name, inventory level, price, max and min values, and company name or machine ID
  - Labels for ID, name, inventory level, price/cost, max and min values, the application title, and company name or machine ID

### Modify Part Form

- **Controls:**
  - Radio buttons for “In-House” and “Outsourced” parts
  - Buttons for “Save” and “Cancel”
  - Text boxes for ID, name, inventory level, price, max and min values, and company name or machine ID
  - Labels for ID, name, inventory level, price, max and min values, the application title, and company name or machine ID

### Add Product Form

- **Controls:**
  - Buttons for “Save,” “Cancel,” “Add” part, and “Delete” part
  - Text boxes for ID, name, inventory level, price, and max and min values
  - Labels for ID, name, inventory level, price, max and min values, and the application
  - A grid view for all parts
  - A grid view for parts associated with the product
  - A “Search” button and a text field with an associated list for displaying the results of the search

### Modify Product Form

- **Controls:**
  - Buttons for “Save,” “Cancel,” “Add” part, and “Delete” part
  - Text boxes for ID, name, inventory level, price, and max and min values
  - Labels for ID, name, inventory level, price, max and min values, and the application “all candidate parts”
  - A grid view for parts associated with the product
  - A “Search” button and a text box with associated list for displaying the results of the search

## Application Functionality

The application includes the following functionalities:

- **Main Form:**
  - Redirect to the “Add Part,” “Modify Part,” “Add Product,” or “Modify Product” forms
  - Delete a selected part or product from the grid view
  - Search for a part or product and display matching results
  - Exit the main form

- **Part Forms:**
  - Add Part Form:
    - Select “In-House” or “Outsourced”
    - Enter name, inventory level, price, max and min values, and company name or machine ID
    - Save the data and then redirect to the main form
    - Cancel or exit out of this form and go back to the main form
  - Modify Part Form:
    - Select “In-House” or “Outsourced”
    - Modify or change data values
    - Save modifications to the data and then redirect to the main form
    - Cancel or exit out of this form and go back to the main form

## Exception Handling

The application includes exception handling for the following conditions:

- Detect non-numeric values in textboxes that expect numeric values
- Ensure Min is less than Max, and Inv is between those two values
- Prevent the user from deleting a product that has a Part associated with it
- Confirm “Delete” actions

## Contributing

Contributions are welcome! Feel free to open issues or pull requests.

## License

This project is licensed under the MIT License.
