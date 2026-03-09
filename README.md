# <p align="center">Ticket Lifestyle & Escalation
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

## Project Summary

This project demonstrates ticket lifecycle management using osTicket within a simulated help desk environment. Tickets were created, assigned priorities and SLAs, escalated, and resolved while observing role-based access and notification behavior.

### Languages Used
- N/A (Web-based configuration)

### Environments Used
- Microsoft Azure
- Remote Desktop
- Windows Server
- Windows 10

### Technologies / Services Used
- osTicket
- Azure Virtual Machines
---

# Demonstration
Started by signing into Azure Portal (portal.azure.com) and navigating to Virtual Machines from the left menu. I selected the virtual machine used for the osTicket setup and opened its Overview page to copy the Public IP address. I then used Remote Desktop (RDP) to connect to the VM with the administrator credentials. Once inside the VM, I opened a web browser and entered http://localhost/osTicket
 in the address bar, which loaded the osTicket setup page. I then followed the installation prompts, entered the help desk information, and configured the MySQL database. After the installation was completed, both the Admin/Agent panel and the End User osTicket portal were available for managing and submitting support tickets.
 
# Scenario 1 – Online Banking System Down (SEV-A)

## Step One: Ticket Created – End User (Karen)
<img src="https://i.postimg.cc/G90VHvVT/01-ticket-online-banking-created-karen.png" width="500">
Logged in End Users osTicket site as the end user Karen and created a new ticket stating that the entire mobile and online banking system was down. The ticket was submitted into the system.

## Step Two: Default Ticket Properties – Agent (John)
<img src="https://i.postimg.cc/V5ypdXpC/02-ticket-online-banking-default-properties-john.png" width="500">
Logged in osTicket Admin/Analyst Login Page as Agent John and opened the ticket. Observed the default priority, department, SLA, and assignment settings before making changes.

## Step Three: SLA & Department Assignment
<img src="https://i.postimg.cc/gr9Qn3Q6/03-ticket-online-banking-sev-a-online-banking.png" width="500">
Edited the ticket properties. Set the Priority from Normal to Emergency, SLA to Sev-A (1 hour, 24/7) and changed the department to Online Banking, then saved the configuration. Notified end user Karen the state of Banking system.

## Step Four: Escalation Behavior
<img src="https://i.postimg.cc/Th8FpnFL/04-ticket-online-banking-inaccessible-john.png" width="500">
Attempted to access the ticket again as John. Observed that the ticket became inaccessible due to department-based permission restrictions after escalation.

## Step Five: Ticket Resolution – Agent (Jane)

<img src="https://i.postimg.cc/vDRkc5kn/05-ticket-online-banking-resolved-by-jane.png" width="500">
Logged in as Agent Jane. Worked the escalated ticket to completion and marked it as resolved before closing the ticket altogether.

---

# Scenario 2 – Adobe Upgrade Request (SEV-B)

## Step One: Ticket Created- End User (Ken)
<img src="https://i.postimg.cc/s1Fqv5qS/06-ticket-adobe-upgrade-created-enduser-ken.png" width="500">
Logged in as the end user Ken and created a ticket stating that the accounting department needed an Adobe upgrade.

## Step Two: SLA & Department Assignment
<img src="https://i.postimg.cc/J7yhHmv3/07-ticket-adobe-upgrade-sev-b-support.png" width="500">
Logged in as Agent John. Checked in with end user Ken before working ticket. Reviewed default properties and set the Priority from Normal to High, SLA to Sev-B (4 hours, 24/7), and assigned the ticket to the Support department.

## Step Three: Ticket Resolution – Agent (John)
<img src="https://i.postimg.cc/VsSN01pR/08-ticket-adobe-upgrade-resolved-by-john.png" width="500">
Assigned the ticket to John. Followed up with end user Ken. Worked the issue to completion and confirmed the issue as resolved before closing ticket.

---
