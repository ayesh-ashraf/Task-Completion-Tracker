# Task Completion Tracker — n8n Automation Workflow

This **n8n workflow** automates task monitoring and notification using **Google Sheets** and **Gmail**.  
It continuously watches a Google Sheet for updates, checks whether tasks are marked as completed, updates their status, and automatically sends an email notification ...saving manual follow-ups and ensuring timely communication.


##  **Purpose**
Manual tracking of completed tasks can easily lead to delays and missed updates.  
This workflow provides an **automated solution** that:
- Detects when a task status changes in a shared Google Sheet.  
- Updates the task record automatically.  
- Sends an instant email notification to the concerned person.  

It’s efficient, simple to deploy, and adaptable to various work environments.

##  **Workflow Overview**
**Workflow Name:** Task Completion Tracker  
**Platform:** n8n  
**Integrated Services:** Google Sheets, Gmail  

##  **Node-by-Node Breakdown**
 **1️⃣ Google Sheets Trigger**  : Starts the workflow automatically whenever any update is made to your Google Sheet. 
 **2️⃣ Get Row(s) in Sheet**  : Reads all rows from the sheet and fetches (brings) the latest task data. 
 **3️⃣ IF** : Condition Check  Verifies whether the “Status” column equals **Completed**. If true, it proceeds to the next step. 
 **4️⃣ Update Row in Sheet** : Updates that particular row, marking that a notification has been sent or a task verified. 
 **5️⃣ Send a Message (Gmail)** : Sends an automated email alert to the relevant person indicating task completion. 

##  **Real-World Use Cases**
This workflow can be customized for many real-life scenarios:
1.  **Team Task Monitoring:** Automatically inform managers when employees complete assigned tasks.  
2.  **Academic Project Tracking:** Notify teachers or supervisors when students finish milestones.  
3.  **Optometry or Clinic Use:** Track follow-ups, patient record updates, or administrative task completions.  
4. **Sales Tracker:** Send automatic notifications when deals are closed or leads converted.  
5.  **Freelancer Updates:** Automatically inform clients when a deliverable is marked as done.  
6.  **Maintenance Teams:** Notify supervisors once a service request is resolved.

##  **Key Benefits**
-  **Time-saving:** Reduces manual checking and reporting.  
-  **Automated Communication:** Ensures no completed task goes unnoticed.  
-  **Real-time Accuracy:** Keeps Google Sheet data up-to-date instantly.  
- **Scalable:** Can be extended for multiple departments or use cases.  

## **Setup Instructions**

### Prerequisites (requirements)
- A Google account with access to Google Sheets and Gmail.  
- An active n8n account (self-hosted or cloud).  
- A properly formatted Google Sheet (columns like: *Task Name*, *Assigned To*, *Status*, *Date*).
### Steps
1. **Create a Google Sheet** with your task list.  
2. **Integrate Google Sheets and Gmail** credentials into n8n.  
3. **Import or recreate the workflow** using the nodes listed above.  
4. **Configure the IF Node Condition**    
5. **Set your Gmail node** to send an email to the intended recipient.  
6. **Activate the Workflow** and test it by updating your Google Sheet.  

##  **Workflow Structure**
Google Sheets Trigger ➜ Get Row(s) in Sheet ➜ IF ➜ Update Row in Sheet ➜ Send a Message (Gmail)

##  **Video Demonstration**

👉 *Watch the workflow in action here:*  
[Watch the demo video here](https://youtu.be/ctg4MFrOSaQ)


## **Author**
Ayesha Ashraf

