# JMeter Performance Testing
## Project Overview
This project contains JMeter performance test collections for two scenarios:
##  Task1 Performance Testing for Booking API
In the scenario Total user: 120000 and Time Period: 12 hours = 12 * 60 * 60 seconds = 43,200 seconds
Throughput (Requests per Second): 120,000 users / 43,200 seconds ≈ 2.78 requests/second
##### Conducted tests in 3 steps:
- 5-minute load test
- 10-minute load test
- 20-minute load test
### Load Test & Throughput Analysis
- Limited the test duration to a maximum of 20 minutes.
- Verified whether the server can handle the expected load.

### This is Load test Step Report 
![load](https://github.com/user-attachments/assets/a3467077-e35c-43b5-bf26-a67aff06d473)


 ### For 5 min Iteration Summary report
 ![5s](https://github.com/user-attachments/assets/4f1eca09-2026-4a37-8d8e-94ae68e18bdd)
 ### For 10 min Iteration Summary report
 ![10new](https://github.com/user-attachments/assets/e2d680bb-7d31-4931-9228-cb0a95f6beff)
 ### For 20 min Iteration statistics from the HTML report
![load html](https://github.com/user-attachments/assets/f46b6958-e33f-47c9-a02a-b8dd2c16e006)

### Stress Test & Bottleneck Identification
After doing a load test for 20 minutes, Gradually increased the load in steps until the server started failing.
### This is stress test Step Report 
![stressss](https://github.com/user-attachments/assets/c1c84968-6327-4e9d-831d-edbf84c3bc89)

### For 4500 user summary report 
![4500](https://github.com/user-attachments/assets/2d9b34b0-fc2c-4351-b092-64702465a062)

### For 5500 user summary report 
![5500](https://github.com/user-attachments/assets/bef04a48-369f-4a46-a769-31e7055cc765)
### For 7500 user summary report 
![7500](https://github.com/user-attachments/assets/3075e99c-5062-4132-aed8-57d6b3c0abc5)
### Stress Test & Bottleneck HTML Report
![html](https://github.com/user-attachments/assets/8589c8e2-4d5c-4692-b061-c931ce8ef7ca)


## load test and stress test from the excel file
[booking-api-test-report.xlsx](https://github.com/user-attachments/files/19252854/booking-api-test-report.xlsx)

# Task 2: Functional Testing for DMoney API
### Summary report
![task2](https://github.com/user-attachments/assets/21ea7aad-db40-4c6e-ae6d-7d94dfc6fd12)
### HTML Report
![task2html](https://github.com/user-attachments/assets/e5c290f1-bf04-4e10-abe0-63a501726e8c)

## Prerequisites
- Apache JMeter (latest version recommended)
- Java 8 or later
- Clone this repository from GitHub
## How to run?
#### Task 1: Running the Booking API Load & Stress Tests
- Open Apache JMeter.
- Load the booking.jmx file.
- Run the test for the required duration.
- View results in the HTML report folder.
####  Task 2: Running the DMoney API Test
- Load the dmoney.jmx file in JMeter.
- Ensure the CSV files (deposit.csv, sendMoney.csv, payment.csv) are placed in the same directory.
- Run the test and validate the response assertions.
##  Notes
booking.jtl dmoney.jtl and the HTML report folder are excluded from GitHub using .gitignore.
