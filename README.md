SQL Temporal Coalescing Algorithms Comparison
Overview
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
Firstly in order to run this you need to have the ability to host a local MySQL server.
For my set up I went with https://dev.mysql.com/downloads/mysql/ and https://downloads.mysql.com/archives/c-cpp/
for the server and command line client.
For the Server you should choose 8.4.3 LTS and the Client just 8.4.0 is fine.
Then once they are downloaded you want to set up your server to the default local hosted port.
Then once you have that up you need to create 3 tables using something like 
CREATE TABLE EmployeeData (
    id CHAR(36) NOT NULL,
    EMP_NO INT NOT NULL,
    Salary INT NOT NULL,
    TSTART DATE NOT NULL,
    END DATE NOT NULL,
    PRIMARY KEY (id)
);
Make sure to name the tables Tempral(Large,Medium,Small)
Then you can run the program and use the insertion page to insert the 3 files into your sql server.
Then you can run the coalecence algorithms.
