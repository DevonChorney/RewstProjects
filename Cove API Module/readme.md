## Requirements

Core integration included by default
Org Variables at the top level organization
cove_partner (This is the Customer ID for your Reseller customer level)
cove_username (The username for your api enabled user)
cove_password (The password for your api enabled user)

## Actions
Cove Backup - Auth - Used for authenticating to the api
Cove Backup - Add User - Used for adding a new user. *Requires SuperUser or Administrator Permissions
Cove Backup - Get User - Returns a specific user
Cove Backup - List Users - Returns an unfiltered list of users
Cove Backup - Get Device - Returns a specific device
Cove Backup - List Devices - Returns an unfiltered list of devices
Cove Backup - Get Customer - Returns a specific customer
Cove Backup - List Customers - Returns an unfiltered list of customers
Cove Backup - List Stale Audit - Returns a list of devices that have not completed a backup in X days. 90 days is the default.
Cove Backup - Billing Report - Returns a report of devices following 2 different billing models. The legacy output for when you are billed in Servers and Workstations only. The DPP model is the newer Cove Data Protection Plan where you are billed for Physicical servers, Virtual servers, and Workstations.


## How do I use this workflow?

### Inputs

All Get actions have multiple input options. Only 1 is required to return data.

### Outputs

All actions return data as taskname.results.output. Within the output is a message and data objects. 

### Triggers

All actions are designed to be used as subworkflows.

### Dragons

Failures will appear to pass but will contain error information within the standard output.
For Security purposes edit the Cove Backup - Auth workflow and redact the body of the Cove_Auth action to prevent leaking your API key.

### Changelog

v1.0 - Initial Commit

### Future Development

Add additional function available through the API that are not documented including recovery testing
Add Office 365 to billing report
Add monitoring options
Add filtering to List actions
