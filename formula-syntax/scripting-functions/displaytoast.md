# DISPLAYTOAST

Display custom text as a toast message. Supported message types are alert, error, info, loading, success, and warning.

### Syntax

```javascript
DISPLAYTOAST.<MESSAGE_TYPE>("<MESSAGE_TEXT>")
```

### Arguments

MESSAGE\_TYPE - Select from ALERT, ERROR, INFO, LOADING, SUCCESS, WARNING.

MESSAGE\_TEXT - Custom message to be displayed.

### Example

```
DISPLAYTOAST.ALERT("The data in this report should not be edited")
DISPLAYTOAST.ERROR("Error fetching data")
DISPLAYTOAST.INFO("2024 Financial Statement - Inforiver")
DISPLAYTOAST.LOADING("Report load in progress")
DISPLAYTOAST.SUCCESS("Report load complete")
DISPLAYTOAST.WARNING("Sensitive data, meant for grade L5 and above only")
```

<figure><img src="../../.gitbook/assets/image (698).png" alt=""><figcaption><p>Alert</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (700).png" alt=""><figcaption><p>Error</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (701).png" alt=""><figcaption><p>Info</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (702).png" alt=""><figcaption><p>Loading</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (703).png" alt=""><figcaption><p>Warning</p></figcaption></figure>
