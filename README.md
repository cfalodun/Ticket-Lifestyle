# <p align="center">Ticket Lifestyle & Escalation
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

## Scenario 1 – Online Banking System Down (SEV-A)

### Step 1: Ticket Created (End User – Karen)
Ticket: **"The entire mobile/online banking system is down."**

<a href="https://postimg.cc/bST35Szq" target="_blank"><img src="https://i.postimg.cc/bST35Szq/01-ticket-online-banking-created-karen.png" alt="01-ticket-online-banking-created-karen"></a>

---

### Step 2: Observe Default Properties (Agent – John)
Observed:
- Priority
- Department
- SLA
- Assigned To

<a href="https://postimg.cc/WqnXyq2N" target="_blank"><img src="https://i.postimg.cc/WqnXyq2N/02-ticket-online-banking-default-properties-john.png" alt="02-ticket-online-banking-default-properties-john"></a>

---

### Step 3: Set Ticket Properties
Configured:
- SLA: **Sev-A (1 hour, 24/7)**
- Department: **Online Banking**

<a href="https://postimg.cc/8fHtYf11" target="_blank"><img src="https://i.postimg.cc/8fHtYf11/03-ticket-online-banking-sev-a-online-banking.png" alt="03-ticket-online-banking-sev-a-online-banking"></a>

---

### Step 4: Access Restriction Behavior
After escalation, the ticket became inaccessible to **John** due to department/SLA restrictions.

<a href="https://postimg.cc/WqnXyq2T" target="_blank"><img src="https://i.postimg.cc/WqnXyq2T/04-ticket-online-banking-inaccessible-john.png" alt="04-ticket-online-banking-inaccessible-john"></a>

---

### Step 5: Ticket Resolution (Agent – Jane)
Ticket worked to completion.

<a href="https://postimg.cc/y3PvG3V6" target="_blank"><img src="https://i.postimg.cc/y3PvG3V6/05-ticket-online-banking-resolved-by-jane.png" alt="05-ticket-online-banking-resolved-by-jane"></a>

---

## Scenario 2 – Adobe Upgrade Request (SEV-B)

### Step 1: Ticket Created (End User)
Ticket: **"Accounting department needs adobe upgrade, broken."**

<a href="https://postimg.cc/640YP495" target="_blank"><img src="https://i.postimg.cc/640YP495/06-ticket-adobe-upgrade-created-enduser-ken.png" alt="06-ticket-adobe-upgrade-created-enduser-ken"></a>

---

### Step 2: Set Ticket Properties
Configured:
- SLA: **Sev-B (4 hours, 24/7)**
- Department: **Support**

<a href="https://postimg.cc/fkNs64wk" target="_blank"><img src="https://i.postimg.cc/fkNs64wk/07-ticket-adobe-upgrade-sev-b-support.png" alt="07-ticket-adobe-upgrade-sev-b-support"></a>

---

### Step 3: Ticket Resolution (Agent – John)
Ticket worked to completion.

<a href="https://postimg.cc/dDYFzMqk" target="_blank"><img src="https://i.postimg.cc/dDYFzMqk/08-ticket-adobe-upgrade-resolved-by-john.png" alt="08-ticket-adobe-upgrade-resolved-by-john"></a>

---

## Scenario 3 – CFO Laptop Failure (SEV-B)
Ticket: **"CFO’s laptop will no longer turn on."**

Configured:
- SLA: **Sev-B (4 hours, 24/7)**
- Department: **Support**

Worked to completion by the assigned agent.

---

## Escalation & Permission Behavior
When tickets were escalated to SEV-A:
- SysAdmins became the final assignment group
- Tickets became inaccessible without proper permissions
- Admin panel access was required to modify visibility

This demonstrates how ticket visibility and modification rights are governed by department and role permissions.

---

## Email Notification Capability
Most ticketing systems (including osTicket) include email notifications.
When a ticket is updated, assigned, or resolved, the end user receives an email and can respond directly.

---

## Real-World Ticket Intake
Tickets can come from phone, chat, email, web forms, or in-person requests.
Even if an issue is fixed immediately, tickets should be created for metrics, documentation, and trend tracking.

---

## Technical Skills Reinforced
- Ticket lifecycle management
- SLA prioritization
- Department routing
- Escalation handling
- Permission-based access control
- Documentation and communication workflow

