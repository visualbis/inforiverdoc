# LEVEL

Returns the row Level in the hierarchy.&#x20;

## Example

We have Region, Country, State and Product Name which denotes each level. The row grand total will be considered as 1st level followed by Region as 2nd level, Country as 3rd Level, State as 4th Level and Product Name as 5th level.

<figure><img src="../../.gitbook/assets/Formula Level.png" alt=""><figcaption><p>Calculating the level</p></figcaption></figure>

For each city, we need to calculate the tax amounts based on level. Using the level formula, we get each hierarchy value and multiply it with the tax% value to arrive at the tax value.

<figure><img src="../../.gitbook/assets/Formula Level 2.png" alt=""><figcaption><p>Using the level column in a calculation</p></figcaption></figure>
