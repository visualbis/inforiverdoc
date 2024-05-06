# FETCH

The FETCH function retrieves data from a URL in real-time. You can pass parameters and keys to extract the specific data.

## Syntax

```javascript
FETCH(URL:string,key:string)
//fetches data from the specified URL
```



## Arguments

URL - String. Required. It is used to specify the URL from which the data has to be fetched.

key- String. Required. It specifies the key whose value is to be extracted.



## Example

In the report below, we have a list of Product IDs. Using the FETCH function we specify the URL, pass the product ID from our report and dynamically retrieve the associated details from a server(API call).&#x20;

Note that we have used the [CONCATENATE ](../text-formatting-functions/concatenate.md)function to concatenate the URL and the Product ID to be passed to fetch the data. To extract the product name, we have used its key "title".

<figure><img src="../../.gitbook/assets/image (652).png" alt=""><figcaption><p>FETCH function</p></figcaption></figure>
