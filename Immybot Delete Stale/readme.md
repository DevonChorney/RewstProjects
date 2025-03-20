## Requirements
Immybot Integration Configured<br />


## How do I use this workflow?

### Inputs

How many days should a device be offline before its consider stale.
Negative number
Defaults to -180 days

### Outputs

"output"
this output contains 2 objects, the list of removed devices and the count of removed devices

### Triggers

Cron scheduled for the 1st of the month

### Dragons

Devices deleted are moved into the deleted tab and can be restored.
Any deleted device is soft deleted.

### Changelog

v1.0 - Initial Commit
