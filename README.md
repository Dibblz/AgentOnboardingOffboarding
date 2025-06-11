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
- Valid credentials stored or handled within PAD.

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
