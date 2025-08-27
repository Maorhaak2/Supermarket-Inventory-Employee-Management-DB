# Supermarket Inventory & Employee Management DB

## Overview
A Python + SQLite system for managing a supermarket chain.  
It tracks **employees, suppliers, products, branches, and activities** (sales and supplies).  
The project is split into three standalone scripts: `initiate.py`, `action.py`, and `printdb.py`.

## Features
- SQLite database (`bgumart.db`) with 5 tables:
  - Employees, Suppliers, Products, Branches, Activities.
- `initiate.py`: creates a fresh database and loads initial data from a config file.
- `action.py`: executes activities (supply or sale) from an actions file.
- `printdb.py`: prints database tables and generates:
  - **Employees report**: name, salary, branch, and sales income.
  - **Activities report**: date, product, quantity, seller/supplier.

## Build & Run
Requirements: Python 3.9+ (no external packages needed)

```bash
# initialize database with configuration
python initiate.py config.txt

# execute activities
python action.py actions.txt

# print tables and reports
python printdb.py
