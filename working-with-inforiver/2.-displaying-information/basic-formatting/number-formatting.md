# Number formatting

Inforiver for Power BI comes prepackaged with _intelligent number formatting & scaling recognition_ capabilities that help display data in a perceptive manner in your table/matrix style reports right out of the box.

## 1. Number scaling

Let us take a sample dataset as shown below. You can immediately spot data of mixed granularity – with values in millions, thousands, and even one that is just a few dollars worth.

<figure><img src="../../../.gitbook/assets/2.4.3.1 Data.png" alt=""><figcaption><p>Data of mixed granularity</p></figcaption></figure>

Let us see how you can handle a dataset of varying granularities & formats using Inforiver.&#x20;

In the Home tab, click on the 'Quick format' dropdown. There are several options, let us look at each of them in detail.

<figure><img src="../../../.gitbook/assets/2.4.1.1 Dropdown menu.png" alt=""><figcaption><p>Number scaling options</p></figcaption></figure>

### a) Measure level scaling

By default, when you assign this data to Inforiver, each measure is formatted using an individual scale. The scaling for each measure is shown in the column header. This is useful to show measures of varying granularities (e.g., Revenue & Quantity) in the same table.

<figure><img src="../../../.gitbook/assets/2.4.1.2 Measure level scaling.png" alt=""><figcaption><p>Measure level scaling</p></figcaption></figure>

### b) Uniform scaling

The 'Uniform' option applies one fixed scale to the entire table and moves the scaling unit display to the header. This is useful when all the measures are of comparable magnitude (e.g., Sales vs Forecast) in the same table.

<figure><img src="../../../.gitbook/assets/2.4.1.3 Uniform scaling.png" alt=""><figcaption><p>Uniform scaling</p></figcaption></figure>

Inforiver automatically chooses the scaling based on the values. But you change it if needed. When you expand the dropdown again, you can see more options. You can select millions, billions, etc. as needed.

<figure><img src="../../../.gitbook/assets/2.4.1.4 Auto Uniform scaling.png" alt=""><figcaption><p>Uniform formatting options</p></figcaption></figure>

### c) Auto scaling

When using the 'auto' option, each cell is formatted individually. In the below image, you can see the suffixes - m and k to denote millions and thousands.

<figure><img src="../../../.gitbook/assets/2.4.1.5 Auto scaling.png" alt=""><figcaption><p>Cell level scaling</p></figcaption></figure>

### d) Native scaling

If you do not want any fancy formatting and need the numbers just as they are in the source data, select the ‘Native’ option.&#x20;

<figure><img src="../../../.gitbook/assets/2.4.1.6 Native scaling.png" alt=""><figcaption><p>Native scaling</p></figcaption></figure>
