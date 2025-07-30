# AgriTech-Documentation


**AgriTech** is a digital platform that focuses on helping smallholder farmers access agricultural machinery in Rwanda. The main purpose is to digitize cooperatives in Rwanda, and by this we will increase farmers' productivity. The system connects four core personas: **Farmers, Cooperative Managers, Extension Officers, and Machine Suppliers**. It also provides a centralized way to manage machine requests, payments, tracking, and maintenance reporting.

### Purpose of AgriTech

Many farmers struggle to access farming machines on time due to manual processes and poor tracking systems. AgriTech solves this by digitizing the entire process, from machine ordering to usage and monitoring, ensuring transparency, traceability, and efficiency for everyone involved.

### Supported users

**Farmers**- They can request for machines from cooperatives and make payments.

**Cooperatives**- They manage machine orders, make payments to machine suppliers, tracking of machines, and lending machines to farmers.

**Extension Officers**- They conduct field visits and update machine conditions.

**Machine Suppliers**- They receive machine requests from cooperatives and supply to them.

### Key features overview

Digital ordering system between farmers, cooperatives, and machine suppliers
IoT machine tracking using GPS and geofencing
Integration with mobile payments
Machinery lending record management
Field reporting by extension officers

AgriTech aims to bring accountability and data-driven decision-making into modern agriculture.


Explore the following sections:

#User Guide
This section outlines how each of our users interacts with the AgriTech platform, from logging in.

Farmers
Key actions:
Place machinery orders to cooperatives
Receive updates from the cooperative
Make payments via mobile money
Step by step
Log in to the mobile app using your phone number.
Navigate to Request machine
Fill out the request form with your preferred machine and duration
Wait for cooperative confirmation
Once notified, make payment
Receive the machine and begin use.
Cooperative Officers
Key Actions:
View farmer machine requests
Contact suppliers to fulfill orders
Manage payments from farmers to suppliers
Record machine arrivals and assign them to farmers
Monitor geofence alerts and machine conditions
Step-by-Step:
Log in to the web-based React dashboard.
View incoming orders in the Orders Panel.
Contact machine suppliers to source the requested machines.
Notify the farmer once availability is confirmed.
Receive payments from the farmer.
Make payments to suppliers.
Upon machine arrival, install IoT tracking devices.
Record the machine in the system and assign it to the requesting farmer.
Monitor machine location and condition reports in real-time.
Receive alerts if a machine exits its geofenced area.
Machine Suppliers
Key Actions:
Confirm machine availability
Deliver machines to cooperatives
Receive payments upon delivery
Step-by-Step:
Log in to your supplier portal.
View machine requests and confirm availability.
Coordinate delivery with the cooperative.
Deliver the machine and mark it as "delivered".
Receive payment from the cooperative.
Extension Officers
Key Actions:
View machines assigned to nearby farmers
Conduct on-site inspections
Update machine condition and status
Add notes or attach images during reports
Step-by-Step:
Open the Extension Officer mobile app.
View your assigned machine list.
Visit each farmer’s location during fieldwork.
Check machine functionality and note any issues.
Update machine status: Working, Needs Maintenance, Broken, etc.
Submit field report
Reports are synced to the system and visible to cooperatives.
Notes
All users have role-based logins and permissions.
Alerts for geofence violations are triggered automatically and shown to cooperatives.
Mobile apps are optimized for offline mode (for fieldwork), with syncing once reconnected.
Machine history and condition logs are accessible to both cooperatives and extension officers.

#FAQ

- Below are some of the most commonly asked questions about using and managing the AgriTech system.

For Farmers
Q1: How do I know if my machine request has been approved? A: You will receive an in-app notification once the cooperative approves your request.

Q2: What payment method is supported? A: We use M-Pesa integration through the Daraja API for all transactions. You’ll be prompted to complete payment from your phone.

Q3: Can I track the machine’s location? A: No, but the cooperative can. They will monitor usage through the tracking system.

For Cooperatives
Q1: How are geofence alerts triggered? A: When a machine leaves its designated area, the IoT device sends a signal to the system, and an alert appears in the dashboard. Q2: Can I update the farmer’s details or reassign machines? A: Yes. From the admin dashboard, go to the “Machinery” section and reassign as needed. Q3: How do I record that a machine has returned? A: Go to the lending record tab and mark the machine as returned manually.

For Machine Suppliers
Q1: How will I know when to supply a machine? A: You’ll get a notification or request through the system once a cooperative places an order. Q2: How do I confirm delivery? A: After delivery, log in and mark the request as “Delivered” in your supplier portal.

For Extension Officers
Q1: Can I update reports offline? A: Yes. The mobile app stores data locally and syncs it once the internet is available. Q2: Can I attach images to my reports? A: Yes. During field reporting, you can upload photos, voice notes, or type notes. Q3: How are reports used? A: Reports are stored in the system and are visible to cooperatives for making decisions about maintenance or retrieval.

General
Q: What if I forget my password? A: Use the “Forgot Password” option on the login screen to reset it via SMS. Q: Can I use this app on any phone? A: The farmer and extension officer apps are optimized for Android and can run on most smartphones. Q: Is AgriTech available in local languages? A: Not yet, but Kinyarwanda support is planned for a future release.

#AI Component

Purpose of AI in AgriTech
In AgriTech, Artificial Intelligence plays a key role in helping cooperatives make smarter, faster, and more informed decisions when sourcing machines from suppliers. Rather than relying on manual judgment or random choices, the AI system analyzes a range of data to recommend the best suppliers based on:

Historical delivery performance
Machine quality and condition reports
Supplier reliability
Timeliness of past deliveries
Extension officer feedback from the field
How It Works
Data Collection The system gathers real-time and historical data from machine records, supplier logs, feedback reports, and IoT tracking history.
Evaluation Model A lightweight AI model (Agentic AI) processes this data to rank suppliers based on machine quality, field performance, and overall reliability.
Recommendation When a cooperative receives a farmer’s request, the AI suggests the top 1–3 suppliers most likely to meet quality, speed, and reliability needs.
Learning Over Time The more data it gathers, the smarter the system gets. For example, if one supplier’s machines consistently break down or arrive late, their ranking is adjusted accordingly.
Future Improvements
In future releases, the AI system may include:

Automated fraud detection in supplier entries
Natural language query handling (e.g., "Find best supplier for dry season")
