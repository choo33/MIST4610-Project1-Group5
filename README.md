Team Name:
Group 5

Team Members:
1. Jason Cho @choo33
2. Victor Montoya @vrm99039

Problem Description:
The Charlotte Padel Club is a growing sports organization focused on managing memberships, court bookings, lessons, and events. They provide various membership plans that differ in price, benefits, and duration. Members can sign up for multiple events the club hosts, reserve courts for their matches, and handle payments. Each member's subscription includes data like plan type, acquisition date, and current status. The club has a dedicated team of staff that oversees operations, organizes events, and builds relationships with sponsors. These sponsors partner with the club to enhance their event promotions and brand visibility.
Our data model is designed to offer an organized way to handle all operational data within a relational database. We aim to support the Charlotte Padel Club in making better business choices while improving both financial and operational efficiency.
<br />
Data Model
<br />
Data Dictionary
<br />
Queries:
1. Query 1 lists the total revenue collected for the current month. It also displays the total for each payment method (e.g., Credit Card, Cash, Online). The results are ordered by total revenue in descending order.
<img width="379" height="177" alt="Screenshot 2025-10-24 at 2 45 55 PM" src="https://github.com/user-attachments/assets/bb76a700-feb3-4998-a793-30902ce05379" />
<img width="280" height="74" alt="Screenshot 2025-10-24 at 2 46 09 PM" src="https://github.com/user-attachments/assets/03d1d0ec-a261-4925-b26a-25ec73ef30b9" />
<br /> Query 1 allows managers to see which payment methods are the most commonly used by members and which methods bring in the most revenue during the current month. This information can help management identify member preferences and help decide which payment options to prioritize or promote. We listed the results in descending order to help management quickly identify the top-performing payment methods, which can influence financial planning in the club.
<br />
2. Query 2 identifies members whose payment amounts exceed the overall average payment across all members. It first finds the average payment using a subquery that retrieves the mean amount from the Payment table. The outer query then lists each qualifying member’s name, payment amount, and payment date. The results are ordered by payment amount in descending order.
<img width="565" height="278" alt="Screenshot 2025-10-24 at 2 53 24 PM" src="https://github.com/user-attachments/assets/f9294de7-248b-40c4-9fb0-80e8bfe85dc3" />
<img width="979" height="602" alt="Screenshot 2025-10-24 at 2 54 08 PM" src="https://github.com/user-attachments/assets/5eca1fa5-d90b-469c-8332-775b27b31063" />
<img width="967" height="260" alt="Screenshot 2025-10-24 at 2 54 20 PM" src="https://github.com/user-attachments/assets/a97bb62f-e0fa-4a79-b43d-e47aca0bcfa3" />
Query 2 allows management to identify high-value members who spend more than the average club member. Recognizing these members is important for maintaining strong relationships and providing loyalty incentives or rewards. Having these insights can also help management find the characteristics of higher-spending members and develop targeted marketing strategies to bring in similar clients. Ordering the results by payment amount makes it easier to see which members contribute the most revenue to the club.
<br />
3. Query 3 lists all active members along with the name of the membership plan each one is enrolled in. It joins the Member, Subscription, and MembershipPlan tables to match members with their current subscriptions and plan names. The results are filtered to include only those with a valid status and are filtered alphabetically by the member's last name.
<img width="572" height="195" alt="Screenshot 2025-10-24 at 3 17 05 PM" src="https://github.com/user-attachments/assets/f6e21184-3653-40ba-a7f9-3117c8051da2" />
<img width="523" height="618" alt="Screenshot 2025-10-24 at 3 17 26 PM" src="https://github.com/user-attachments/assets/2393cb9e-b474-4089-b0b5-668e1427acb5" />
<img width="511" height="587" alt="Screenshot 2025-10-24 at 3 17 39 PM" src="https://github.com/user-attachments/assets/3449f7b3-9c7f-4466-9814-ee9ae439b52e" />
<img width="490" height="590" alt="Screenshot 2025-10-24 at 3 17 51 PM" src="https://github.com/user-attachments/assets/9d51350f-dab8-4729-9580-84bf2b30213e" />
<img width="567" height="589" alt="Screenshot 2025-10-24 at 3 18 07 PM" src="https://github.com/user-attachments/assets/8428198e-8bba-446b-8794-14feb0529167" />
<img width="516" height="585" alt="Screenshot 2025-10-24 at 3 18 43 PM" src="https://github.com/user-attachments/assets/c7ef4bff-41b7-4c9d-aaa0-b9c0ebdd699d" />
<img width="545" height="589" alt="Screenshot 2025-10-24 at 3 18 58 PM" src="https://github.com/user-attachments/assets/3ebe9eb2-7a38-43df-b7f5-0e987d95f17a" />
<img width="478" height="66" alt="Screenshot 2025-10-24 at 3 19 08 PM" src="https://github.com/user-attachments/assets/ac51a2ee-4d00-46bc-bb74-e447060f9930" />
Query 3 enables managers to quickly view all current active members and which membership plans they belong to. It's useful for finding which plans are the most popular and to verify active memberships within the club. Sorting by last name makes it easy to locate a member. 

<br />

4. Query 4
Revenue Analysis by Membership Plan with Active Member Count
DESCRIPTION: This query calculates total monthly revenue, average billing amount, and count of active members for each membership plan type.
JUSTIFICATION: Management needs to understand which membership plans generate the most revenue and attract the most members. This helps with pricing strategy, marketing focus, and resource allocation decisions.
COMPLEXITY FEATURES: Multiple table JOIN, GROUP BY, Built-in functions (SUM, AVG, COUNT)
<img width="674" height="347" alt="image" src="https://github.com/user-attachments/assets/ab2d0a30-943b-44df-8a7f-d9b88978a52b" />
<img width="674" height="224" alt="image" src="https://github.com/user-attachments/assets/1fe89b20-f4af-4c2c-b2a3-45653bd62a93" />

<br />

5. Query 5
Payment Timeliness and Billing Status by Member
Description: This query identifies each member’s most recent billing record, total amount billed, and whether their last payment was made on time. It helps detect members who might have recurring billing issues or delays in payments.
Justification: From a managerial perspective, this query is essential for monitoring member payment reliability. It can be used to identify delinquent accounts, automate reminder notices, and improve cash flow prediction.
Complexity Features: Multiple JOINs, aggregation, subquery, date comparison, and conditional logic (CASE).
<img width="725" height="349" alt="image" src="https://github.com/user-attachments/assets/74c05464-5da0-4c04-bb61-165e2425b3fe" />
<img width="441" height="433" alt="image" src="https://github.com/user-attachments/assets/4355fcee-d3df-436d-a99d-1e4ca5b9dd40" />
<img width="441" height="433" alt="image" src="https://github.com/user-attachments/assets/95fb791d-d5ba-4e4c-9762-222fddbdef4f" />
<img width="441" height="433" alt="image" src="https://github.com/user-attachments/assets/40748077-73c9-4bb8-ae69-85613fa8f7ba" />
<img width="441" height="425" alt="image" src="https://github.com/user-attachments/assets/bb30c043-333d-4d59-b586-55ac8aa0ec87" />
<br />
6. Query 6
Member Engagement by Membership Plan
Description: This query shows how engaged members are based on their membership plan type by calculating the average number of events attended for each membership plan type.
Justification: Managers can use this to determine which membership plans encourage more  participation in club activities. Plans with low engagement may need improved benefits or  promotional events to increase member involvement.
Complexity Features: Multiple table JOINs, GROUP BY, aggregate functions (COUNT, AVG), and calculated fields.
<img width="933" height="296" alt="image" src="https://github.com/user-attachments/assets/fa7537f1-fb55-483f-8674-737a89b8bd12" />
<img width="664" height="341" alt="image" src="https://github.com/user-attachments/assets/c9fe10c1-7835-41a4-842e-82538055ffee" />

<br />
7. Query 7:
Staff Event Management Performance Overview
Description: This query summarizes how many events each staff member managed and the total number of attendees across all their events.
Justification: This is useful for management to evaluate staff workload and performance, recognize top-performing event coordinators, and optimize event assignments.
Complexity Features: Multiple table JOINs, aggregation, and GROUP BY with calculated fields.
<img width="615" height="249" alt="image" src="https://github.com/user-attachments/assets/52051af0-352f-4fe8-a8b3-424ca13b3f04" />
<img width="615" height="155" alt="image" src="https://github.com/user-attachments/assets/919b06a0-96f4-4a74-b000-0803882e9e89" />

<br />














