# NORMSDIST

The NORMSDIST function calculates the standard normal distribution for a measure, with a mean of 0 and a standard distribution of 1.

<pre class="language-javascript"><code class="lang-javascript"><strong>normsdist(value, cumulative)
</strong></code></pre>

## Arguments

value - The measure for which to calculate the normal distribution. This is a required argument.

cumulative - If cumulative is TRUE, NORMDIST returns the cumulative distribution function; if cumulative is FALSE, it returns the probability mass function.&#x20;

## Example

```javascript
NORMSDIST([InterestRate], TRUE)
```

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Standard normal distribution</p></figcaption></figure>
