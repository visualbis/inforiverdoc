# LOGGEDIN\_EMAIL

The LOGGEDIN\_EMAIL  identifier returns the user email ID. It can be used along with a SETVALUE function to capture the user who updates a data input field.&#x20;

## Example

The Last Updated At and Last Updated By housekeeping fields can be used to capture the user and time at which a data input field was updated. These fields however cannot be written back. Instead of using the built-in housekeeping columns, you can leverage the SETVALUE function with the LOGGEDIN\_EMAIL  identifier and store the email ID in a text field.

In this example, we're capturing the user email ID when the status single select field is changed. The text fields can then be written back to the preferred destination(s).

<figure><img src="../../.gitbook/assets/image (1359).png" alt=""><figcaption><p>Capture the email ID using the SETVALUE function</p></figcaption></figure>
