# NORMDIST

The NORMDIST function calculates the normal distribution for a measure, mean and standard deviation.

## Syntax

<pre class="language-javascript"><code class="lang-javascript"><strong>normdist(value, mean, stddev, cumulative)
</strong></code></pre>

## Arguments

value - The measure for which to calculate the normal distribution. This is a required argument.

mean - The arithmetic mean of the distribution. This is a required argument.

stddev - The standard deviation of the distribution. This is a required argument.

cumulative - If cumulative is TRUE, NORMDIST returns the cumulative distribution function; if cumulative is FALSE, it returns the probability mass function.&#x20;

## Example

```javascript
NORMDIST(42, 40, 1.5, TRUE)
```

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Normal distribution </p></figcaption></figure>
