# <p align="center">Ticket Lifecycle & Escalation (osTicket)</p>
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

---

## Project Summary

This project demonstrates ticket lifecycle management using osTicket within a simulated help desk environment hosted in Microsoft Azure. The lab showcases how tickets are created, assigned priorities and SLAs, escalated across departments, and resolved by different agents based on role-based access control. It highlights how support teams manage incidents efficiently while maintaining proper workflow, communication, and escalation procedures.

---

## Environments Used

- Microsoft Azure  
- Windows Server  
- Windows 10  
- Remote Desktop (RDP)  

---

## Technologies Used

- osTicket  
- Azure Virtual Machines  

---

# Demonstration

---

## Accessing the osTicket Environment

1. Log into the Azure Portal  
2. Navigate to Virtual Machines  
3. Select the VM hosting osTicket  
4. Copy the Public IP Address  
5. Connect using Remote Desktop (RDP)  
6. Open a web browser inside the VM and go to:

7. Log into:
   - Admin/Agent Panel (for ticket management)  
   - End User Portal (for ticket creation)  

---

# Scenario 1 – Online Banking System Down (SEV-A)

---

## Step 1 – Ticket Created (End User: Karen)

1. Log into the End User Portal  
2. Create a new ticket  
3. Enter issue:
   - "Entire mobile and online banking system is down"  
4. Submit the ticket  

<img src="https://i.postimg.cc/G90VHvVT/01-ticket-online-banking-created-karen.png" width="500">

---

## Step 2 – Default Ticket Properties (Agent: John)

1. Log into the Admin/Agent Panel  
2. Open the ticket as John  
3. Review:
   - Priority  
   - Department  
   - SLA  
   - Assignment  

<img src="https://i.postimg.cc/V5ypdXpC/02-ticket-online-banking-default-properties-john.png" width="500">

---

## Step 3 – SLA & Department Assignment

1. Edit the ticket properties  
2. Set:
   - Priority → Emergency  
   - SLA → Sev-A (1 hour, 24/7)  
   - Department → Online Banking  
3. Save the changes  
4. Notify the end user  

<img src="https://i.postimg.cc/gr9Qn3Q6/03-ticket-online-banking-sev-a-online-banking.png" width="500">

---

## Step 4 – Escalation Behavior

1. Attempt to access the ticket again as John  
2. Observe:
   - The ticket is no longer accessible  
   - Access is restricted due to department reassignment  

<img src="https://i.postimg.cc/Th8FpnFL/04-ticket-online-banking-inaccessible-john.png" width="500">

---

## Step 5 – Ticket Resolution (Agent: Jane)

1. Log in as Jane  
2. Open the escalated ticket  
3. Work the issue to completion  
4. Mark the ticket as Resolved  
5. Close the ticket  

<img src="https://i.postimg.cc/vDRkc5kn/05-ticket-online-banking-resolved-by-jane.png" width="500">

---

# Scenario 2 – Adobe Upgrade Request (SEV-B)

---

## Step 1 – Ticket Created (End User: Ken)

1. Log into the End User Portal  
2. Create a new ticket  
3. Enter issue:
   - "Accounting department needs an Adobe upgrade"  
4. Submit the ticket  

<img src="https://i.postimg.cc/s1Fqv5qS/06-ticket-adobe-upgrade-created-enduser-ken.png" width="500">

---

## Step 2 – SLA & Department Assignment (Agent: John)

1. Log into the Admin/Agent Panel  
2. Open the ticket  
3. Review default properties  
4. Set:
   - Priority → High  
   - SLA → Sev-B (4 hours, 24/7)  
   - Department → Support  
5. Save changes  

<img src="https://i.postimg.cc/J7yhHmv3/07-ticket-adobe-upgrade-sev-b-support.png" width="500">

---

## Step 3 – Ticket Resolution (Agent: John)

1. Assign the ticket to John  
2. Follow up with the end user  
3. Complete the request  
4. Mark the ticket as Resolved  
5. Close the ticket  

<img src="https://i.postimg.cc/VsSN01pR/08-ticket-adobe-upgrade-resolved-by-john.png" width="500">
