# Inforiver Writeback Matrix pre-requisites

To set up Inforiver enterprise, two additional steps must be completed in collaboration with the Power BI administrator.

* Since Inforiver is an add-on visual that operates on top of the Power BI framework, users must log in with their Microsoft O365 account. [Admin consent](admin-consent-for-inforivers-entra-id/) will be required to log in, add writeback destinations, or connect to integrations like Teams or SharePoint.
* Network firewalls block connections from IP addresses that do not have permission. [Whitelist Inforiver’s outbound IPs in your Azure SQL database firewall rules.](whitelist-inforiver-ips.md)
