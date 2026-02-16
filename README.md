# <p align="center">Ticket Lifestyle
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

## Objective

Simulate real-world help desk workflows by:

- Creating tickets as end users  
- Observing and modifying ticket properties as agents  
- Assigning SLAs and departments  
- Escalating tickets  
- Resolving tickets to completion  
- Understanding role-based access control  

---

# Scenario 1 – Online Banking System Down (SEV-A)

## Step 1: Ticket Created (End User – Karen)

Ticket:
"The entire mobile/online banking system is down."

![Online Banking Ticket Created](https://i.postimg.cc/bST35Szq/01-ticket-online-banking-created-karen.png)

---

## Step 2: Observe Default Properties (Agent – John)

Observed:
- Priority  
- Department  
- SLA  
- Assigned To  

![Default Properties](https://i.postimg.cc/WqnXyq2N/02-ticket-online-banking-default-properties-john.png)

---

## Step 3: Set Ticket Properties

Configured:
- SLA: **Sev-A (1 hour, 24/7)**  
- Department: **Online Banking**  

![Sev-A Configuration](https://i.postimg.cc/8fHtYf11/03-ticket-online-banking-sev-a-online-banking.png)

---

## Step 4: Access Restriction Behavior

After escalation, the ticket became inaccessible to John due to department/SLA restrictions.

![Inaccessible Ticket](https://i.postimg.cc/WqnXyq2T/04-ticket-online-banking-inaccessible-john.png)

Admin permissions were required to regain visibility.

---

## Step 5: Ticket Resolution (Agent – Jane)

Ticket worked to completion.

![Resolved Ticket](https://i.postimg.cc/y3PvG3V6/05-ticket-online-banking-resolved-by-jane.png)

---

# Scenario 2 – Adobe Upgrade Request (SEV-B)

## Step 1: Ticket Created (End User)

Ticket:
"Accounting department needs Adobe upgrade, broken."

![Adobe Ticket Created](https://i.postimg.cc/640YP495/06-ticket-adobe-upgrade-created-enduser-ken.png)

---

## Step 2: Set Ticket Properties

Configured:
- SLA: **Sev-B (4 hours, 24/7)**  
- Department: **Support**

![Adobe Sev-B Configuration](https://i.postimg.cc/fkNs64wk/07-ticket-adobe-upgrade-sev-b-support.png)

---

## Step 3: Ticket Resolution (Agent – John)

Ticket worked to completion.

![Adobe Resolved](https://i.postimg.cc/dDYFzMqk/08-ticket-adobe-upgrade-resolved-by-john.png)

---

# Scenario 3 – CFO Laptop Failure (SEV-B)

Ticket:
"CFO’s laptop will no longer turn on."

Configured:
- SLA: **Sev-B (4 hours, 24/7)**  
- Department: **Support**

Ticket worked to completion by the assigned agent.

---

# Escalation & Permission Behavior

When tickets were escalated to SEV-A:

- SysAdmins became the final assignment group  
- Tickets became inaccessible without proper permissions  
- Admin panel access was required to modify visibility  

This demonstrates how ticket visibility and modification rights are governed by department and role permissions.

---

# Email Notification Capability

Most ticketing systems (including osTicket) include automated email notifications.

Each time a ticket is:
- Updated  
- Assigned  
- Commented on  
- Resolved  

The end user receives an email notification and can respond directly.

---

# Real-World Ticket Intake

Tickets may originate from:

- Phone calls  
- Chat applications  
- Email  
- Web forms  
- In-person requests  

Even if an issue is resolved immediately, tickets should be created for:

- Performance tracking  
- SLA metrics  
- Documentation  
- Trend analysis  

Everything should be logged.

---

# Technical Skill Development

This lab reinforces:

- Ticket lifecycle management  
- SLA prioritization  
- Department routing  
- Escalation handling  
- Permission-based access control  
- Professional documentation practices  

Repeating this lab builds operational confidence and structured troubleshooting skills.
