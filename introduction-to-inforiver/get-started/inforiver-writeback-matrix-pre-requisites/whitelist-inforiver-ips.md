# Whitelist Inforiver IPs

Inforiver's outbound IP address must be whitelisted in the customer's network or database firewalls to access Inforiver services.&#x20;

{% hint style="info" %}
Inforiver IP addresses to be whitelisted:

i) 20.80.81.140 - 20.80.81.143&#x20;

ii) 172.170.162.240
{% endhint %}

### 1. Whitelisting Inforiver for On-Prem Writeback

Inforiver writeback may be unable to connect to on-prem databases hosted in data centers or office networks. This happens because the network firewall between your database and Inforiver blocks the inbound communication initiated for writeback.&#x20;

For writeback to work with on-prem databases, the admin must whitelist the 5 Inforiver outbound IPs in the network firewall.

### 2. Whitelisting for Azure SQL

Azure SQL destinations have firewall rules that block connections originating from non-whitelisted IPs. To connect to Azure SQL databases from Inforiver, you must create a firewall rule to open the firewall for a specific range of IP addresses. [Learn more about creating firewall rules.](https://learn.microsoft.com/en-us/azure/azure-sql/database/firewall-create-server-level-portal-quickstart?view=azuresql)

Follow the steps in the image below to whitelist the 5 Inforiver outbound IP addresses.&#x20;

<figure><img src="../../../.gitbook/assets/image (9) (7).png" alt=""><figcaption><p>Creating firewall rules</p></figcaption></figure>

The screengrab below shows the firewall rules configured for Inforiver would.

<figure><img src="../../../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Firewall rules configured for Inforiver</p></figcaption></figure>
