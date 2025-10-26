Team Name:
Group 5

Team Members:
1. Jason Cho @choo33
2. Victor Montoya @vrm99039
3. Vivi Correa @vivi-correa
4. Aritra Bhattacharya @aritrabha1
5. Soham Joshi @sohamjoshiii

Problem Description:
The Charlotte Padel Club is a growing sports organization focused on managing memberships, court bookings, lessons, and events. They provide various membership plans that differ in price, benefits, and duration. Members can sign up for multiple events the club hosts, reserve courts for their matches, and handle payments. Each member's subscription includes data like plan type, acquisition date, and current status. The club has a dedicated team of staff that oversees operations, organizes events, and builds relationships with sponsors. These sponsors partner with the club to enhance their event promotions and brand visibility.
Our data model is designed to offer an organized way to handle all operational data within a relational database. We aim to support the Charlotte Padel Club in making better business choices while improving both financial and operational efficiency.
<br /> <br />
Data Model <br />
<img width="1954" height="1550" alt="image" src="https://github.com/user-attachments/assets/78561643-cb58-4ca0-bbc4-600b458b28fc" />
<br /> <br />
Data Dictionary <br />
<img width="825" height="621" alt="image" src="https://github.com/user-attachments/assets/49763fc6-36e1-49eb-a0d4-dcf510aef718" />
<img width="437" height="546" alt="image" src="https://github.com/user-attachments/assets/ba8c1394-435c-49aa-8438-00d0ce8d05f0" />
<img width="614" height="209" alt="image" src="https://github.com/user-attachments/assets/8fc10634-7134-4ebe-84a5-28313040450d" />
<img width="712" height="458" alt="image" src="https://github.com/user-attachments/assets/073563cd-c8bf-416e-8568-7dcb57fc8489" />
<img width="716" height="434" alt="image" src="https://github.com/user-attachments/assets/3238ee3b-3c77-40dc-bd5f-31696ba86a12" />
<img width="735" height="498" alt="image" src="https://github.com/user-attachments/assets/cd8e8da5-2c15-447d-983b-b7a2a9b8fad2" />
<img width="735" height="623" alt="image" src="https://github.com/user-attachments/assets/26d03045-1653-4622-a44b-c2f2e2b1cf41" />
<img width="603" height="622" alt="image" src="https://github.com/user-attachments/assets/89eb55d1-bc75-4351-a8e7-014fa0d4eff5" />
<img width="727" height="666" alt="image" src="https://github.com/user-attachments/assets/16c9ada2-8e90-4fa7-ac07-839d0619d3a9" />
<img width="755" height="571" alt="image" src="https://github.com/user-attachments/assets/fec50979-3576-4797-a43d-f364585ac105" />
<img width="730" height="314" alt="image" src="https://github.com/user-attachments/assets/8da82cbe-f5e5-4a54-bbeb-77ff89be0b4c" />
<img width="714" height="369" alt="image" src="https://github.com/user-attachments/assets/70fa2b4f-b606-4280-b8b0-7eacec61dc5c" />
<br /> <br />
Queries:
1. Query 1 lists the total revenue collected for the current month. It also displays the total for each payment method (e.g., Credit Card, Cash, Online). The results are ordered by total revenue in descending order.
<img width="379" height="177" alt="Screenshot 2025-10-24 at 2 45 55 PM" src="https://github.com/user-attachments/assets/bb76a700-feb3-4998-a793-30902ce05379" />
<img width="280" height="74" alt="Screenshot 2025-10-24 at 2 46 09 PM" src="https://github.com/user-attachments/assets/03d1d0ec-a261-4925-b26a-25ec73ef30b9" />
<br /> Query 1 allows managers to see which payment methods are the most commonly used by members and which methods bring in the most revenue during the current month. This information can help management identify member preferences and help decide which payment options to prioritize or promote. We listed the results in descending order to help management quickly identify the top-performing payment methods, which can influence financial planning in the club.
<br /> <br />
2. Query 2 identifies members whose payment amounts exceed the overall average payment across all members. It first finds the average payment using a subquery that retrieves the mean amount from the Payment table. The outer query then lists each qualifying member’s name, payment amount, and payment date. The results are ordered by payment amount in descending order.
<img width="565" height="278" alt="Screenshot 2025-10-24 at 2 53 24 PM" src="https://github.com/user-attachments/assets/f9294de7-248b-40c4-9fb0-80e8bfe85dc3" />
<img width="979" height="602" alt="Screenshot 2025-10-24 at 2 54 08 PM" src="https://github.com/user-attachments/assets/5eca1fa5-d90b-469c-8332-775b27b31063" />
<img width="967" height="260" alt="Screenshot 2025-10-24 at 2 54 20 PM" src="https://github.com/user-attachments/assets/a97bb62f-e0fa-4a79-b43d-e47aca0bcfa3" />
Query 2 allows management to identify high-value members who spend more than the average club member. Recognizing these members is important for maintaining strong relationships and providing loyalty incentives or rewards. Having these insights can also help management find the characteristics of higher-spending members and develop targeted marketing strategies to bring in similar clients. Ordering the results by payment amount makes it easier to see which members contribute the most revenue to the club.
<br /> <br />
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
<br /> <br />
4. Query 4
Revenue Analysis by Membership Plan with Active Member Count
<br /> Description: This query calculates total monthly revenue, average billing amount, and count of active members for each membership plan type.
<br /> Justification: Management needs to understand which membership plans generate the most revenue and attract the most members. This helps with pricing strategy, marketing focus, and resource allocation decisions.
<br /> Complexity Features: Multiple table JOIN, GROUP BY, Built-in functions (SUM, AVG, COUNT)
<img width="674" height="347" alt="image" src="https://github.com/user-attachments/assets/ab2d0a30-943b-44df-8a7f-d9b88978a52b" />
<img width="674" height="224" alt="image" src="https://github.com/user-attachments/assets/1fe89b20-f4af-4c2c-b2a3-45653bd62a93" />
<br /> <br />
5. Query 5
Payment Timeliness and Billing Status by Member
<br /> Description: This query identifies each member’s most recent billing record, total amount billed, and whether their last payment was made on time. It helps detect members who might have recurring billing issues or delays in payments.
<br /> Justification: From a managerial perspective, this query is essential for monitoring member payment reliability. It can be used to identify delinquent accounts, automate reminder notices, and improve cash flow prediction.
<br /> Complexity Features: Multiple JOINs, aggregation, subquery, date comparison, and conditional logic (CASE).
<img width="725" height="349" alt="image" src="https://github.com/user-attachments/assets/74c05464-5da0-4c04-bb61-165e2425b3fe" />
<img width="441" height="433" alt="image" src="https://github.com/user-attachments/assets/4355fcee-d3df-436d-a99d-1e4ca5b9dd40" />
<img width="441" height="433" alt="image" src="https://github.com/user-attachments/assets/95fb791d-d5ba-4e4c-9762-222fddbdef4f" />
<img width="441" height="433" alt="image" src="https://github.com/user-attachments/assets/40748077-73c9-4bb8-ae69-85613fa8f7ba" />
<img width="441" height="425" alt="image" src="https://github.com/user-attachments/assets/bb30c043-333d-4d59-b586-55ac8aa0ec87" />
<br /> <br />
6. Query 6
Member Engagement by Membership Plan
<br /> Description: This query shows how engaged members are based on their membership plan type by calculating the average number of events attended for each membership plan type.
<br /> Justification: Managers can use this to determine which membership plans encourage more  participation in club activities. Plans with low engagement may need improved benefits or  promotional events to increase member involvement.
<br /> Complexity Features: Multiple table JOINs, GROUP BY, aggregate functions (COUNT, AVG), and calculated fields.
<img width="933" height="296" alt="image" src="https://github.com/user-attachments/assets/fa7537f1-fb55-483f-8674-737a89b8bd12" />
<img width="664" height="341" alt="image" src="https://github.com/user-attachments/assets/c9fe10c1-7835-41a4-842e-82538055ffee" />
<br /> <br />
7. Query 7:
Staff Event Management Performance Overview
<br /> Description: This query summarizes how many events each staff member managed and the total number of attendees across all their events.
<br /> Justification: This is useful for management to evaluate staff workload and performance, recognize top-performing event coordinators, and optimize event assignments.
<br /> Complexity Features: Multiple table JOINs, aggregation, and GROUP BY with calculated fields.
<img width="615" height="249" alt="image" src="https://github.com/user-attachments/assets/52051af0-352f-4fe8-a8b3-424ca13b3f04" />
<img width="615" height="155" alt="image" src="https://github.com/user-attachments/assets/919b06a0-96f4-4a74-b000-0803882e9e89" />
<br /> <br />
8. Query 8
<br /> Active subscribers with 0 events attended
<br /> What it shows: Active subscribers who have never attended an event.
<br /> Why it helps: Flags disengaged members for onboarding nudges, welcome events, or targeted offers to increase retention.
<img width="1230" height="950" alt="image" src="https://github.com/user-attachments/assets/00492131-25a9-4503-ae53-c4080dddbbd6" />
<img width="1230" height="880" alt="image" src="https://github.com/user-attachments/assets/95a44911-deed-4eef-9fcd-6b402dde51a3" />
<img width="790" height="238" alt="image" src="https://github.com/user-attachments/assets/16b49b4e-726d-49bf-8ca9-8d28247acc54" />
<br /> <br />
9. Query 9
<br /> Number of payments and total paid for each active member 
<br /> What it shows: For each active member, the number of payments and total paid to date.
<br /> Why it helps: Quickly surfaces high-value members and those with low payment activity for retention/upsell efforts.
<img width="1104" height="1004" alt="image" src="https://github.com/user-attachments/assets/85d7be40-8b40-4741-90d8-34d9be604779" />
<img width="1052" height="990" alt="image" src="https://github.com/user-attachments/assets/8915c93c-a99c-45d6-b698-0d36aa2135d5" />
<img width="1052" height="1012" alt="image" src="https://github.com/user-attachments/assets/36239e7d-1ff2-47be-a595-00118ef45e76" />
<img width="1052" height="1012" alt="image" src="https://github.com/user-attachments/assets/a7eb850e-bfc5-4acc-bd53-0074bbd70980" />
<img width="1052" height="1012" alt="image" src="https://github.com/user-attachments/assets/7b53b502-4df6-47a1-979a-343f838dd708" />
<img width="1052" height="1012" alt="image" src="https://github.com/user-attachments/assets/a6620aac-360b-4246-a5aa-3ab6c8485361" />
<img width="1052" height="1012" alt="image" src="https://github.com/user-attachments/assets/7a3885fa-cb49-4cb5-94d1-5357127380e7" />
<img width="1052" height="760" alt="image" src="https://github.com/user-attachments/assets/963da606-eabf-478e-8799-cad77b0a1f90" />
<br /> <br />
10. Query 10
<br /> Payment channel profitability
<br /> What it shows: For each payment method (like Credit Card, Cash, Online), this query displays the total revenue collected, number of transactions, and average payment amount across all payments in the system.
<br /> Why it helps: Gives management a clear view of which payment channels are most used and most profitable, helping them decide which payment options to prioritize, promote, or streamline in the club’s financial system.
<img width="736" height="432" alt="image" src="https://github.com/user-attachments/assets/c8e01725-d25b-44e9-9adf-a741e236a0ec" />
<img width="736" height="152" alt="image" src="https://github.com/user-attachments/assets/e357f54f-a755-4e8c-88eb-b7d483e5a22e" />
<br /> <br />

Query Checklist:
<br /> 
<img width="2032" height="306" alt="image" src="https://github.com/user-attachments/assets/c71c713b-4267-48dc-8939-4a86eebb278a" />

































