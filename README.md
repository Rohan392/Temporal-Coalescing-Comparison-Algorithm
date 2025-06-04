SQL Temporal Coalescing Algorithms Comparison

**Overview**
A comparative analysis tool for evaluating the performance of two temporal coalescing algorithms using SQL and .NET. Designed to visualize, test, and benchmark algorithm performance across different datasets.

**Features**
- Benchmarking large datasets for runtime, memory usage, and edge-case handling.
- Interactive UI for visualizing and comparing coalesced time intervals.
- Modular .NET design focused on extensibility and performance testing.

**Technologies**
- SQL Server
- C# (.NET)
- Windows Forms / WPF

**Database Tables **
CREATE TABLE EmployeeData (

    id CHAR(36) NOT NULL,
    EMP_NO INT NOT NULL,
    Salary INT NOT NULL,
    TSTART DATE NOT NULL,
    END DATE NOT NULL,
    PRIMARY KEY (id)
);

**Instructions for Running the Program:**

Step 1:
- Install [the MySQL C/C++ Command Line Client (version 8.4.0) from the MySQL Archives.] (https://dev.mysql.com/downloads/mysql/ and https://downloads.mysql.com/archives/c-cpp/)
- Ensure both the server and client versions are compatible and correctly installed on your system.

Step 2: Configure the MySQL Server
- Set up your MySQL server to run on the default localhost port (3306).
- Start the MySQL service and ensure that it is running without errors.

Step 3: Create Required Tables
- Open your MySQL Command Line Client or preferred GUI (e.g., MySQL Workbench), and execute the following SQL command to create a base table:

CREATE TABLE EmployeeData (
    id CHAR(36) NOT NULL,
    EMP_NO INT NOT NULL,
    Salary INT NOT NULL,
    TSTART DATE NOT NULL,
    END DATE NOT NULL,
    PRIMARY KEY (id)
);
- You will need three separate tables, named exactly:
    - TempralLarge
    - TempralMedium
    - TempralSmall
- Each of these tables should use the same schema as shown above.

Step 4:
- Run the Application
- Launch the application executable.
- Navigate to the insertion page within the UI.
- Use this interface to upload the three data files into your MySQL tables.

Step 5: 
- Execute the Coalescing Algorithms
- Once the data has been successfully inserted, return to the main page or algorithm section of the application.
- Select and run the temporal coalescing algorithms on the datasets.
- Results (performance metrics, visualizations, etc.) will be displayed through the UI.
