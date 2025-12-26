---
Collaboration and SharePoint Automation
Overview
This repository documents practical work delivered across Microsoft 365 collaboration services, with a focus on SharePoint automation, governance, and operational reliability. Each entry reflects real engineering tasks that improved consistency, security, and lifecycle management within the collaboration stack.
---
1. SharePoint Automation
Automated Secure Deletion of SharePoint Soft Delete Bin
Summary:  
Developed a PowerShell automation using a dedicated service account and the PnP PowerShell module to clear a SharePoint site’s soft delete bin every 24 hours. This was implemented to meet stricter document security requirements and ensure that deleted content did not remain accessible beyond the organization’s defined retention expectations.
Key Actions:
• Created a service account with scoped permissions for the target SharePoint site.
• Wrote a PowerShell script using PnP PowerShell to identify and remove items from the soft delete bin.
• Validated script behavior in a controlled environment before production rollout.
• Ensured the script aligned with existing retention and compliance policies.
Impact:  
Provided a predictable, automated method for enforcing secure deletion requirements and reduced manual administrative overhead.
---
Operationalized Automation with Windows Task Scheduler
Summary:  
Configured Windows Task Scheduler to run the SharePoint cleanup script every 24 hours using the service account. This ensured consistent execution without requiring manual intervention.
Key Actions:
• Created a scheduled task configured to run under the service account.
• Set the task to execute the PowerShell script on a daily interval.
• Implemented logging to track successful runs and identify failures.
• Validated that the task executed reliably over multiple cycles.
Impact:  
Established a stable, automated operational workflow that ensured the cleanup process ran consistently and aligned with security requirements.
---
2. Collaboration Governance
Microsoft Bookings Deployment
Summary:  
Worked with a customer to design and deploy a Microsoft Bookings solution that supported their scheduling workflow. Built a shared mailbox, configured delegate permissions, and established a centralized process for handling appointment requests.
Key Actions:
• Coordinated with the customer to understand scheduling needs and operational requirements.
• Created a dedicated shared mailbox to support Bookings notifications.
• Assigned appropriate delegate permissions for staff responsible for managing requests.
• Configured the Bookings page to route all appointment activity through the shared mailbox.
• Validated the end‑to‑end workflow from user booking to staff response.
Impact:  
Delivered a structured, reliable scheduling solution that centralized communication and improved the customer’s ability to manage appointment requests.
