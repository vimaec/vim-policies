# Business Continuity and Disaster Recovery (BC/DR) Plan

**Policy Owner:** VIMBuild, LLC  
**Author:** Martin Ashton  
**Effective Date:** 02/06/2025

## Purpose
The purpose of this business continuity plan is to prepare VIMBuild, LLC in the event of service outages caused by factors beyond our control (e.g., natural disasters, man-made events), and to restore services to the widest extent possible in a minimum time frame.

## Scope
All VIMBuild, LLC IT systems that are business critical. This policy applies to all employees of VIMBuild, LLC and to all relevant external parties, including but not limited to VIMBuild, LLC consultants and contractors.

The following scenarios are excluded from the BC/DR plan scope:
- Loss of availability for a production hosting service provider (Microsoft Azure)

In the event of a loss of availability of a hosting service provider, the driver of response will confer with the executive staff to determine an appropriate response strategy.

## Policy

### Disaster Recovery and Business Continuity
In the event of a major disruption to production services and a disaster affecting the availability and/or security of the VIMBuild, LLC office, senior managers and executive staff shall determine mitigation actions.

A disaster recovery test, including a test of backup restoration processes, shall be performed on an annual basis.

Continuity of information security shall be considered along with operational continuity.

In the case of an information security event or incident, refer to the [Incident Response Plan](./incident_response_plan.md).

### Communications and Escalation
Executive staff and senior managers should be notified of any disaster affecting VIMBuild, LLC facilities or operations.

Communications shall take place over any available regular channels including Slack, Teams, emails, text messaging, and phone calls.

## Roles and Responsibilities

| Role | Responsibility |
|------|--------------|
| [Administrator](./roles.md#administrator) | Leads BC/DR efforts to mitigate losses and recover the corporate network and information systems. Coordinates external and client communications. Ensures continuity of customer-facing services. |
| [Department Heads](./roles.md#department-heads) | Responsible for communication with staff and continuity of business functions. |

## Continuity of Critical Services
Procedures for maintaining continuity of critical services in a disaster can be found in **Appendix A**.

Recovery Time Objectives (RTO) and Recovery Point Objectives (RPO) can be found in **Appendix B**.

### Strategy for Maintaining Continuity
| Key Business Process | Continuity Strategy |
|----------------------|--------------------|
| Customer (Production) Service Delivery | Rely on Microsoft Azure availability commitments and SLAs. |
| Email | Utilize Microsoft 365 and Microsoft's SLAs. |
| Finance, Legal, HR | Vendor-hosted SaaS applications. |
| Sales and Marketing | Vendor-hosted SaaS applications. |

## Plan Activation
This BC/DR shall be automatically activated in the event of the loss or unavailability of any of the VIMBuild, LLC remote offices, or a natural disaster (i.e., severe weather, regional power outage, earthquake) affecting the business region.

## Appendix A - Business Continuity Procedures by Scenario

### Employee Remote Home Office Offline (Power and/or Network)
- Relocate to alternative office location with power and network connectivity (30-60 minutes)
- Verify telephony, CRM, & email connectivity at alternative office location (10 minutes)
- Resume normal operations remotely

### SaaS Tools Down
- **Intercom Down**: Notify customers, use email, activate Excel spreadsheet case tracking
- **Email Down**: Use alternate email accounts, manually manage cases
- **Teams Down**: Use alternate services (Zoom, Slack)

## Appendix B - RTOs/RPOs
| Rank | Asset Affected | Business Impact | Owners | RTO | RPO | Comments/Gaps |
|------|--------------|----------------|--------|-----|-----|---------------|
| 1 | Microsoft Azure Datacenters | Core services | [Administrator](./roles.md#administrator) | Microsoft SLA | Microsoft SLA | |
| 2 | Employee Remote Office | Inability to access data | [Administrator](./roles.md#administrator) + Affected Employee(s) | 60 mins minimum |  |  |
