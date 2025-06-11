# AgentOnboardingOffboarding

# FirefoxAgentNewHire2 – Agent Onboarding Automation

## Overview

This Power Automate Desktop flow automates the onboarding process of a new agent by extracting data from a ServiceNow ticket and provisioning accounts across three systems:

- **Salesforce**
- **OneLogin**
- **Agent Hierarchy Portal**

## Functionality

- Parses required agent information directly from an open ServiceNow ticket in the browser.
- Automates form population and submission in Salesforce to create the agent account.
- Creates the corresponding user account in OneLogin with appropriate attributes.
- Updates the Agent Hierarchy system to reflect the new agent's presence and reporting structure.

## Prerequisites

- Power Automate Desktop installed and configured.
- Access to:
  - ServiceNow (ticket view)
  - Salesforce (agent creation permissions)
  - OneLogin (admin portal)
  - Agent Hierarchy system (write access)

## How to Run

1. Open the ServiceNow ticket in a browser window.
2. Launch the flow from Power Automate Desktop.
3. The flow will automatically:
   - Extract the ticket data
   - Open each target system
   - Create the agent in all three platforms

##  Notes

- Ensure pop-up blockers are disabled for all related websites.
- Recommended browsers: Edge or Chrome with browser automation extensions enabled.
- Errors in ticket formatting may result in partial or failed automation.
- Must be recently logged into all systems

------------------------------------------------------------------------------------

# AgentTermination – Agent Offboarding Automation

## Overview

This Power Automate Desktop flow automates the deactivation of agent accounts across three platforms, using data from a ServiceNow ticket:

- **Salesforce**
- **OneLogin**
- **Agent Hierarchy Portal**

## Functionality

- Extracts agent identifiers and relevant data from an open ServiceNow ticket.
- Navigates to each system and deactivates the agent's account using appropriate workflows or admin panels.

## Prerequisites

- Power Automate Desktop installed and configured.
- Access to:
  - ServiceNow (ticket view)
  - Salesforce (admin access)
  - OneLogin (admin access)
  - Agent Hierarchy system (edit permissions)

## How to Run

1. Open the ServiceNow ticket in a browser window.
2. Launch the flow from Power Automate Desktop.
3. The flow will:
   - Parse the agent info
   - Log into each system
   - Deactivate or disable the agent’s account in all three systems

## Notes

- Be sure that the ticket contains complete agent information to avoid skipped systems.
- Confirmation dialogs may appear during some steps—monitor for interruptions if running in attended mode.
- All systems must be accessible from the host machine.
- Must be recently logged into all systems






