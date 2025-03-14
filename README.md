# JMeter Performance Testing
## Project Overview
This project contains JMeter performance test collections for two scenarios:
## Performance Testing for Booking API
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
![load](https://github.com/user-attachments/assets/f2f066e9-25bc-4aba-a610-267bbffc1015)

 ### For 5 min Iteration Summary report
 ![5s](https://github.com/user-attachments/assets/4f1eca09-2026-4a37-8d8e-94ae68e18bdd)
 ### For 10 min Iteration Summary report
 ![10new](https://github.com/user-attachments/assets/e2d680bb-7d31-4931-9228-cb0a95f6beff)
 ### For 20 min Iteration statistics from the HTML report
![load](https://github.com/user-attachments/assets/ad3644ae-be5c-4856-b78c-2108b3ca204b)
### Stress Testing 
After doing a load test for 20 minutes, we will now slowly perform a user stress test for 20 minutes.
### This is Stress Testing Step report 
![stressss](https://github.com/user-attachments/assets/038ff878-51a8-4d2e-89c8-b1ea00fff622)


## Dmoney Transaction
### S






## Technology I used:
- Postman
- Newmman
- Report: newman-html-extra
## How to run?
- Clone this project
- Collect .env from developer and put on the source root folder
- Hit following command:
  - ``` npm i ```
  - ``` npm test ```
- Report will be generated in Reports folder!
