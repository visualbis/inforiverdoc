# SETCFRULE

You can enable or disable conditional formatting rules using this function. Note that the rule should already have been created to be able to refer to it in the function.

### Syntax

```javascript
SETCFRULE(CFRULE.RULE_NAME, BOOLEAN_ARG)
```

### Arguments

RULE\_NAME – The name of the conditional formatting rule to be set.

BOOLEAN\_ARG - Set to TRUE to enable the rule. Set to FALSE to disable the rule.

### Example

```
SETCFRULE(CFRULE.[Data Bars - Profit], TRUE) #Enables the data bar rule set for sales
SETCFRULE(CFRULE.[Sequential - Sales], FALSE) #Disables the data bar rule set for sales
SETCFRULE(CFRULE.[Sequential - Sales], THIS) #Disables the data bar rule set for sales
```

<figure><img src="../../.gitbook/assets/image (400).png" alt=""><figcaption><p>Set conditional formatting rule</p></figcaption></figure>
