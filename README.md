Team Name:
Group 5

Team Members:
1. Jason Cho @choo33

Problem Description

Data Model

Data Dictionary

Queries:
1. Query 1 lists the total revenue collected for the current month. It also displays the total for each payment method (e.g., Credit Card, Cash, Online). The results are ordered by total revenue in descending order.
<img width="379" height="177" alt="Screenshot 2025-10-24 at 2 45 55 PM" src="https://github.com/user-attachments/assets/bb76a700-feb3-4998-a793-30902ce05379" />
<img width="280" height="74" alt="Screenshot 2025-10-24 at 2 46 09 PM" src="https://github.com/user-attachments/assets/03d1d0ec-a261-4925-b26a-25ec73ef30b9" />
Query 1 allows managers to see which payment methods are the most commonly used by members and which methods bring in the most revenue during the current month. This information can help management identify member preferences and help decide which payment options to prioritize or promote. We listed the results in descending order to help management quickly identify the top-performing payment methods, which can influence financial planning in the club.

2. Query 2 identifies members whose payment amounts exceed the overall average payment across all members. It first finds the average payment using a subquery that retrieves the mean amount from the Payment table. The outer query then lists each qualifying member’s name, payment amount, and payment date. The results are ordered by payment amount in descending order.
<img width="565" height="278" alt="Screenshot 2025-10-24 at 2 53 24 PM" src="https://github.com/user-attachments/assets/f9294de7-248b-40c4-9fb0-80e8bfe85dc3" />
<img width="979" height="602" alt="Screenshot 2025-10-24 at 2 54 08 PM" src="https://github.com/user-attachments/assets/5eca1fa5-d90b-469c-8332-775b27b31063" />
<img width="967" height="260" alt="Screenshot 2025-10-24 at 2 54 20 PM" src="https://github.com/user-attachments/assets/a97bb62f-e0fa-4a79-b43d-e47aca0bcfa3" />
