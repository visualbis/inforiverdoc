# Inforiver Writeback Matrix April 2025 - v4.4.2

This release includes the following fixes:

#### **1. Inserting rows and measures with filter context in connected planning**

Both Inforiver and Infobridge can support filter context, allowing for seamless connected planning even while using slicers in either or both of the connected visuals.

Let's consider the example below:

* A source visual in a bridge has three row dimensions: _Country, Category_ and _SubCategory._

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption><p>Source visual in the bridge</p></figcaption></figure>

* The connecting visual has only two row dimensions: _Category_ and _SubCategory_ with the _Country_ dimension added as a slicer to filter data based on country.&#x20;

<figure><img src="../.gitbook/assets/image (1392).png" alt=""><figcaption><p>Connecting visual</p></figcaption></figure>

While integrating these visuals results in a mismatch in dimension mapping, Inforiver allows you to map the additional source row (or measure) to the connecting visual's filter dimension.&#x20;

First, we will enable filter context in the above visual using Inforiver Super Filter.

<figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption><p>Setting up filter context using Super Filter visual</p></figcaption></figure>

During integration, the additional filter dimension is displayed, allowing the visuals to be integrated.

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption><p>Filter dimension mapped</p></figcaption></figure>

Previously, if the filter dimension is a row (as in the example above), you could insert only rows from the bridge source and vice versa. With this update, you can now insert both rows and measures from the bridge source to the connected visual, regardless of whether your filter context dimension is a row or a measure.

<figure><img src="../.gitbook/assets/image (1412).png" alt=""><figcaption><p>Inserted rows and measures from the source via the bridge</p></figcaption></figure>

#### **2. Missing Infobridge Writeback data in Azure SQL destination - for reports with more than 75 records**

In the AWS environment, when Inforiver reports containing more than 75 records were written back via Infobridge, the writeback data was not present in the Azure SQL destination—even though the writeback was reported as successful. This issue has now been resolved.

#### **3. Unable to delete a cell value in text measure - resets to default value**

When a cell value in a text measure was deleted, it reverted to its default value rather than showing an empty cell. This bug has been fixed.
