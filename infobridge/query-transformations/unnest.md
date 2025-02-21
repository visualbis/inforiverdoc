---
description: >-
  Learn how to use the Unnest transformation to convert delimited values into
  separate rows and flatten your data.
---

# Unnest

## Using the Unnest transformation to flatten your data

You can leverage the **Unnest** transformation to flatten your data. For instance, when you have multi-select options or comma-separated text values in your report, you can split your values into multiple rows.

Let's look at an example to demonstrate how the Unnest function works. Consider a table that captures the orders placed. The investment products purchased by each customer are separated by commas.

<figure><img src="../../.gitbook/assets/image (6) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Orders table</p></figcaption></figure>

An account manager may need to add details specific to each investment instrument, like an interest rate. They would need each product in a separate row to enter the rates as shown below. This is where the Unnest function can be used.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Flattened data</p></figcaption></figure>

Let's look at this Inforiver report that contains a multi-select data input field with benchmarks.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Inforiver report with multi-select options</p></figcaption></figure>

After importing the report into Infobridge and removing the Quarter column, let's apply the Unnest transformation. Choose Benchmark as the target column and comma as the delimiter.

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Unnest transformation in Infobridge</p></figcaption></figure>

Notice how each benchmark is flattened into a separate row. You can perform operations like creating a conditional column to set a rate for each benchmark.

<figure><img src="../../.gitbook/assets/image (1135) (1).png" alt=""><figcaption><p>Output of Unnest transformation</p></figcaption></figure>
