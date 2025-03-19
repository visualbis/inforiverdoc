# Inforiver Writeback Matrix - March 2025 - v4.2.

The bug fixes that are deployed as part of this release have been listed below:

### Migration:

* The migration issue causing column header misalignment after upgrading to a new version has been rectified in the current release.

### Infobridge:

* Cell-level formulas were not being captured in Infobridge in some cases like source refreshes. The issue where edited cells with applied formulas appeared as null in the query has been fixed.
* It was observed that rows inserted from Infobridge were sporadically failing to load in target reports. This has been rectified.

### Scenarios:

* Simulations run on formula measures that refer to forecast, data input, and native measures were not retained in scenarios. In the latest version,  &#x20;simulations on formula measures will be intact when switching between scenarios.
* The values in visual columns that were appearing as 0 in scenarios will now be captured accurately.
