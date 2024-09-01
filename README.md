# Mini Grocery Stall Management System

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [System Requirements](#system-requirements)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Menu Options](#menu-options)
7. [Data Structure](#data-structure)
8. [Contributing](#contributing)
9. [License](#license)

## Introduction

The Mini Grocery Stall Management System is an assembly language program designed to manage inventory, sales, and reporting for a small grocery stall. This system provides a user-friendly interface for viewing and managing inventory, processing sales, and generating reports.

## Features

- View current inventory
- Restock items
- Process sales transactions
- Sort inventory by stock count
- Generate sales reports
- Color-coded low stock warnings

## System Requirements

- x86 compatible processor
- DOS or DOS emulator
- MASM (Microsoft Macro Assembler) or compatible assembler

## Installation

1. Clone this repository or download the `Mini Grocery Stall Management System.asm` file.
2. Assemble the code using MASM or a compatible assembler:
   ```
   masm Mini Grocery Stall Management System.asm;
   link Mini Grocery Stall Management System.obj;
   ```
3. Run the resulting executable:
   ```
   Mini Grocery Stall Management System.exe
   ```

## Usage

Upon running the program, you will be presented with a main menu. Use the number keys to navigate through the options and follow the on-screen prompts to perform various operations.

## Menu Options

1. **View Inventory**: Displays the current inventory, including item IDs, names, quantities, and prices. Items with low stock (5 or fewer) are highlighted in red.

2. **Restock Item**: Allows you to add more stock to a specific item. You'll be prompted to enter the item ID and the quantity to restock.

3. **Sell Items**: Processes a sale transaction. You'll need to enter the item ID and the quantity sold. The system will update the inventory and sales records accordingly.

4. **Sort Items**: Provides options to view items that are in stock (more than 5 units) or low/out of stock (5 or fewer units).

5. **Sales Report**: Generates a detailed report of sales, including quantities sold and total revenue for each item.

0. **Exit the Program**: Closes the application.

## Data Structure

The program uses the following data structure for inventory management:

- `inventory`: An array containing item information (ID, name, quantity, price)
- `sales`: An array tracking the quantity sold for each item
- `item_price`: An array storing the price of each item
