# LOGGEDIN\_NAME

The LOGGEDIN\_NAME identifier returns the user name. It can be used along with a SETVALUE function to capture the user who updates a data input field.&#x20;

## Example

The Last Updated At and Last Updated By housekeeping fields can be used to capture the user and time at which a data input field was updated. These fields however cannot be written back. Instead of using the built-in housekeeping columns, you can leverage the SETVALUE function with the LOGGEDIN\_NAME identifier and store the user name in a text field.

In this example, we're capturing the user name when the approval checkbox is changed. The text fields can then be written back to the preferred destination(s).

<figure><img src="../../.gitbook/assets/image (1360).png" alt=""><figcaption><p>Capturing the user name with the SETVALUE function</p></figcaption></figure>
