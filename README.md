# SQL Temporal Coalescing Algorithms Comparison

---

**Contributors:**  
- [Malcolm Todd](https://github.com/Rubixue)  

---

## Overview

A comparative analysis tool for evaluating the performance of two temporal coalescing algorithms using SQL and .NET. Designed to visualize, test, and benchmark algorithm performance across different datasets.

---

## Features

- Benchmarking large datasets for runtime, memory usage, and edge-case handling.  
- Interactive UI for visualizing and comparing coalesced time intervals.  
- Modular .NET design focused on extensibility and performance testing.

---

## Technologies

- SQL Server  
- C# (.NET)  
- Windows Forms / WPF  

---

## Instructions for Running the Program

### Step 1: Install Dependencies  
- Install [MySQL C/C++ Command Line Client (version 8.4.0)](https://dev.mysql.com/downloads/mysql/) from the MySQL Archives.  
- Ensure both server and client versions are compatible and correctly installed.

### Step 2: Configure MySQL Server  
- Set up your MySQL server to run on the default localhost port (3306).  
- Start the MySQL service and ensure it runs without errors.

### Step 3: Create Required Tables  
- Open your MySQL Command Line Client or GUI (e.g., MySQL Workbench).  
- Execute the following SQL to create the base table schema:

```sql
CREATE TABLE EmployeeData (
    id CHAR(36) NOT NULL,
    EMP_NO INT NOT NULL,
    Salary INT NOT NULL,
    TSTART DATE NOT NULL,
    END DATE NOT NULL,
    PRIMARY KEY (id)
);
