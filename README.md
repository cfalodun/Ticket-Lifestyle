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
- Windows Server
- Windows 10

### Technologies / Services Used
- osTicket
- Active Directory (integration context)
- Azure Virtual Machines
---

# Demonstration

# Scenario 1 – Online Banking System Down (SEV-A)

## Ticket Created – End User (Karen)

"The entire mobile/online banking system is down."

<img src="https://i.postimg.cc/G90VHvVT/01-ticket-online-banking-created-karen.png" width="500">

---

## Default Ticket Properties – Agent (John)

Observed:
- Priority
- Department
- SLA
- Assigned To

<img src="https://i.postimg.cc/V5ypdXpC/02-ticket-online-banking-default-properties-john.png" width="500">

---

## SLA & Department Assignment

Configured:
- SLA: **Sev-A (1 hour, 24/7)**
- Department: **Online Banking**

<img src="https://i.postimg.cc/gr9Qn3Q6/03-ticket-online-banking-sev-a-online-banking.png" width="500">

---

## Escalation Behavior

After escalation, the ticket became inaccessible due to permission restrictions tied to department and SLA configuration.

<img src="https://i.postimg.cc/Th8FpnFL/04-ticket-online-banking-inaccessible-john.png" width="500">

Admin access was required to grant visibility.

---

## Ticket Resolution – Agent (Jane)

<img src="https://i.postimg.cc/vDRkc5kn/05-ticket-online-banking-resolved-by-jane.png" width="500">

---

# Scenario 2 – Adobe Upgrade Request (SEV-B)

## Ticket Created – End User

"Accounting department needs Adobe upgrade, broken."

<img src="https://i.postimg.cc/s1Fqv5qS/06-ticket-adobe-upgrade-created-enduser-ken.png" width="500">

---

## SLA & Department Assignment

Configured:
- SLA: **Sev-B (4 hours, 24/7)**
- Department: **Support**

<img src="https://i.postimg.cc/J7yhHmv3/07-ticket-adobe-upgrade-sev-b-support.png" width="500">

---

## Ticket Resolution – Agent (John)

<img src="https://i.postimg.cc/VsSN01pR/08-ticket-adobe-upgrade-resolved-by-john.png" width="500">

---

# Scenario 3 – CFO Laptop Failure (SEV-B)

Ticket:
"CFO’s laptop will no longer turn on."

Configured:
- SLA: **Sev-B (4 hours, 24/7)**
- Department: **Support**

Worked to completion by assigned agent.

---
