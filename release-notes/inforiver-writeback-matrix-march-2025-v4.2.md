# Inforiver Writeback Matrix - March 2025 - v4.2.

The bug fixes that are deployed as part of this release have been listed below:

### Column header alignment:

* The column headers were misaligned when the report had a single column dimension in the measure on rows layout. The alignment issue has been rectified.

### Infobridge:

* Cell-level formulas were not being captured in Infobridge in some cases like source refreshes. The issue where edited cells with applied formulas appeared as null in the query has been fixed.
* It was observed that rows inserted from Infobridge were sporadically failing to load in target reports. This has been rectified.

### Scenarios:

* Simulations run on formula measures that refer to forecast, data input, and native measures were not retained in scenarios. In the latest version,  &#x20;simulations on formula measures will be intact when switching between scenarios.
* The values in visual columns that were appearing as 0 in scenarios will now be captured accurately.
