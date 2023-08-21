# HYPERLINK

The HYPERLINK function returns hyperlinked text which will navigate to a given URL.&#x20;

## Syntax

```javascript
hyperlink(link:string, value:string)
```

## Arguments

link - A text string containing the URL to navigate to.

value - The hyperlinked text description that will be displayed in the report.

## Example

```javascript
hyperlink('http://Inforiver.com', 'Inforiver')
```

Returns “Inforiver” as hyperlinked text to navigate the URL 'http://www.Inforiver.com'. On clicking the hyperlinked text, a dialog box prompts for permission to navigate to the URL. Click on the OK button to open the webpage in the browser.
