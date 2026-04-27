# Power Automate IT Helpdesk Ticketing System

## Overview


This is a lightweight IT helpdesk ticketing system built using Power Automate and SharePoint Lists.

The focus of this project is on workflow automation, trigger behavior, and debugging, rather than UI development. SharePoint Lists are used as both the data source and input interface, with no Power Apps frontend.


**Architecture**
- SharePoint List (IT_Tickets) as the data store
- Power Automate for workflow logic
- Outlook for notifications

**Basic flow:**

User submits ticket → Flow triggers → Processing logic → SharePoint updates → Notifications sent

<br>

**Flows Implemented**

**1. New Ticket Notification**
- Handles ticket creation events
- Updates ticket metadata
- Sends confirmation and assignment notifications

**2. Critical Ticket Escalation**
- Monitors ticket updates
- Applies conditional logic for high-priority scenarios
- Triggers escalation and updates ticket state

**3. Resolved Ticket Notification**
- Detects resolution state changes
- Updates resolution metadata
- Notifies the requester

<br>

**Testing Approach**

Flows were tested in isolation to ensure predictable behavior:

- Enabled one flow at a time
- Used controlled test data (different priorities and statuses)
- Verified SharePoint updates and email outputs
- Reviewed run history to confirm execution paths

Results:

- All flows executed successfully
- No duplicate notifications observed
- Trigger behavior worked as expected

<br>

**Future Improvements / Refactor Plan**

- Refactor logic into more structured and scalable flow design
- Improve branching and control flow handling
- Explore more dynamic assignment logic
- Enhance maintainability and readability of flows

<br>

> [!NOTE]
> This project is intentionally kept simple to focus on core Power Automate concepts and real-world workflow behavior.
> Screenshots of the overall setup are included for reference, covering the SharePoint list structure, flow list overview in Power Automate, and sample email outputs from
> testing.

<br>
🙋Created by Mark Thomas Bundang| | https://github.com/tab8
