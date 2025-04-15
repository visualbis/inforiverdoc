# Notes

Notes are static text added to a data point or visual to give some descriptive details.&#x20;

{% embed url="https://lumel.wistia.com/medias/2a56qcku4i" %}
Notes - Overview
{% endembed %}

Observe that notes do not have options for a reply and do not capture time stamps.&#x20;

<figure><img src="../../.gitbook/assets/8.1.1 Notes.png" alt=""><figcaption><p>Notes in Inforiver</p></figcaption></figure>

You can insert notes at a cell level, row/column header level, as notes column, and as footnotes.

<figure><img src="../../.gitbook/assets/8.1.2 Notes.png" alt=""><figcaption><p>Data level notes</p></figcaption></figure>

Inforiver also provides an option to add notes at the report level as shown below.

<figure><img src="../../.gitbook/assets/Report level notes.png" alt=""><figcaption><p>Report level notes</p></figcaption></figure>

In reports with large number of hierarchies, you can see notes rolled up at the subtotal and grand total level even if the hierarchies are collapsed. This enables executives to see collapsed and summarized reports but still see exception notes rolled up at the parent levels.

<figure><img src="../../.gitbook/assets/Roll up notes (1).png" alt=""><figcaption><p>Roll-up notes</p></figcaption></figure>

{% hint style="info" %}
* You can [export](../10.-exporting-reports/export/) notes along with the report in Excel and PDF. You can also [write back](../12.-data-writeback/) to databases, shared drives, or URLs.
* Notes added in reading mode will not be saved to the base report. Report users can however export notes.
{% endhint %}

Notes configuration options are shown:

<figure><img src="../../.gitbook/assets/image (1197).png" alt=""><figcaption><p>Notes configurations</p></figcaption></figure>

{% hint style="warning" %}
Notes will not be retained when switching between layouts. For example, notes added in the Measure on Rows layout will not be available if you change the layout to default.
{% endhint %}

## 1. Cell-level notes

1.1. Let's see how to add notes. Click on a cell, click 'Notes', and then 'Add new note'.

{% hint style="info" %}
To add the same note for multiple cells, Ctrl + click to select each cell, then add a note.
{% endhint %}

<figure><img src="../../.gitbook/assets/8.1.3 Notes.png" alt=""><figcaption><p>Adding a new note</p></figcaption></figure>

1.2. An editor opens where you can add hyperlinks and apply rich formatting. Enter a note as shown below.

<figure><img src="../../.gitbook/assets/8.1.4 Notes.png" alt=""><figcaption><p>Notes editor</p></figcaption></figure>

1.3. Try out the formatting options as shown below. Click 'Save'.

<figure><img src="../../.gitbook/assets/8.1.5 Notes.png" alt=""><figcaption><p>Applying rich formatting</p></figcaption></figure>

1.4. You can see an indicator and as you hover over it, you can see the note.

<figure><img src="../../.gitbook/assets/8.1.6 Notes.png" alt=""><figcaption><p>Notes is visible on hover</p></figcaption></figure>

1.5. All the notes added to the report can be seen in one place. Click  'Notes' and 'View all notes' from the dropdown. The cell-level notes can be seen in the 'All' tab.

<figure><img src="../../.gitbook/assets/8.1.6(2) Notes.png" alt=""><figcaption><p>Cell level note in the notes panel</p></figcaption></figure>

1.6. You may need to enter a note that applies to multiple cells, for example, a particular marketing strategy may have contributed to the increase in sales for specific regions and quarters. You can select a series of cells and add a single note that applies to all of them.

<figure><img src="../../.gitbook/assets/3.1. Single note gif.gif" alt=""><figcaption><p>Single note for multiple cells</p></figcaption></figure>

## 2. Header-level notes

2.1. To add a note at the row or column header level, select the row/column. Click on the 'Notes' icon. A side panel opens providing a large screen editor.

<figure><img src="../../.gitbook/assets/8.1.7 Header notes.png" alt=""><figcaption><p>Header level notes</p></figcaption></figure>

2.2. Enter the note. Let's now change the color of the notes indicator. Click on a different color from the bottom of the side panel.

<figure><img src="../../.gitbook/assets/8.1.8 Header notes.png" alt=""><figcaption><p>Changing the indicator color</p></figcaption></figure>

2.3. You also have the option to select a custom color for the indicator. Click on the multicolored icon as highlighted in the image.

<figure><img src="../../.gitbook/assets/8.1.9 Header notes.png" alt=""><figcaption><p>Custom color for note indicator</p></figcaption></figure>

2.4. In addition to the formatting options available for cell-level notes, you also have numbered/bulleted lists. Click 'Save'.

<figure><img src="../../.gitbook/assets/8.1.10 Header notes.png" alt=""><figcaption><p>Adding numbered/bulleted lists</p></figcaption></figure>

2.5. Header-level notes are visible both in the side panel and on hover.

<figure><img src="../../.gitbook/assets/8.1.11 Header notes.png" alt=""><figcaption><p>Header-level notes</p></figcaption></figure>

2.6. Similarly, select a row and add a note. You can edit/delete the note using the corresponding icons on the right.

<figure><img src="../../.gitbook/assets/8.1.11(2) Header notes.png" alt=""><figcaption><p>Row category note</p></figcaption></figure>

## 3. Report-level notes

With Inforiver, you can also add notes and explanations at the report level as shown below.

3.1. Click on 'Notes' and then 'Report Summary'. In the 'Report Summary' side panel, enter the note.

<figure><img src="../../.gitbook/assets/Report level notes 1.png" alt=""><figcaption><p>Report level note</p></figcaption></figure>

3.2. On clicking 'Save', the note gets displayed in the side panel. You can edit/delete the note by clicking on the corresponding icon in the top right.

<figure><img src="../../.gitbook/assets/Report level notes 2.png" alt=""><figcaption><p>Report level notes added</p></figcaption></figure>

## 4. Roll-up notes

If you add a note at the leaf node level in a hierarchical data structure, the notes will automatically roll up to the total/subtotal level even when the leaf nodes are collapsed. To configure roll-up notes, in 'Settings' -> turn on the 'Roll-up indicator' toggle as shown in the below image and click 'Apply'.

<figure><img src="../../.gitbook/assets/Roll up notes.png" alt=""><figcaption><p>Roll-up indicator</p></figcaption></figure>

In the below image, notes have been added at the sub region level. By clicking on the rollup indicator at the region level, you can see the consolidated notes.

<figure><img src="../../.gitbook/assets/Roll up notes 2.png" alt=""><figcaption><p>Rolled up notes</p></figcaption></figure>

## 5. Footnotes

Notes can be viewed as footnotes are an integral part of financial statements and provide supplementary information such as the accounting method used or an explanation of important financial results.&#x20;

To enable footnotes, in the 'Notes' dropdown, turn on the 'Footnote' toggle. You can see the footnotes as highlighted.

<figure><img src="../../.gitbook/assets/8.1.14 Footnotes.png" alt=""><figcaption><p>Footnotes</p></figcaption></figure>

## 6. Notes column

Row-level notes can be added in a separate column.&#x20;

6.1. Enable the **Notes Column** toggle from the Notes dropdown menu.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Notes column option</p></figcaption></figure>

6.2. A notes column gets added. Double-click on a cell and start typing in the rich text editor. You can apply formatting such as bold, italic, underline, font/background color, and hyperlinks.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Adding notes</p></figcaption></figure>

6.3. You can delete a particular note in the Notes column by hovering over it and clicking the ![](https://docs.inforiver.com/~gitbook/image?url=https%3A%2F%2F3062809325-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FEbkCXCUXmtUq5tcnUtZE%252Fuploads%252FvMIIiGPx2KnaU92ZpPSQ%252Fimage.png%3Falt%3Dmedia%26token%3D750c9e29-6f91-48fa-b676-80672a88a2f0\&width=30\&dpr=4\&quality=100\&sign=3bb3eb66\&sv=2)icon.

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Deleting notes</p></figcaption></figure>

## 7. Hide notes

7.1. To hide the footnotes, turn off the footnote toggle.

7.2. To hide the notes column, turn off the notes column toggle.

7.3. To hide the cell, header, and report-level notes, turn on the 'Hide all notes' toggle. Note that by using this option, all the notes including the footnotes and notes column are hidden.&#x20;

<figure><img src="../../.gitbook/assets/8.1.15 Hide notes.png" alt=""><figcaption><p>Hiding all notes</p></figcaption></figure>

## 8. Settings

You can customize the notes indicator, position, footnote height, and more.&#x20;

8.1. Click on 'Settings' from the 'Notes' dropdown.

<figure><img src="../../.gitbook/assets/8.1.18 Settings.png" alt=""><figcaption><p>Customization options for notes</p></figcaption></figure>

8.2. A dialog box opens. The default selections are shown in the below image.

<figure><img src="../../.gitbook/assets/8.1.19 Settings.png" alt=""><figcaption><p>Default settings for notes</p></figcaption></figure>

8.3. There are a number of indicator types such as numbered, lettered, arrow, etc. Indicators can also be resized. By default, indicators are to the left of the cell. We have made changes to the default settings and the result is shown in the below image.

<figure><img src="../../.gitbook/assets/8.1.22 Settings.png" alt=""><figcaption><p>Changes made to the indicators and footnotes</p></figcaption></figure>

The notes indicator can be set at the report level (as shown above), in which case all notes in a report would have the same indicator. You can set individual indicators for each note as well.

<figure><img src="../../.gitbook/assets/image (10) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Notes indicator</p></figcaption></figure>

## 9. Marker mode

Marker Mode can be used to highlight important observations during presentations. Markings are temporary and can be cleared.&#x20;

9.1. In the Notes dropdown, click the **Marker Mode** option.

<figure><img src="../../.gitbook/assets/image (1198).png" alt=""><figcaption><p>Marker mode option</p></figcaption></figure>

9.2. A marker icon is enabled on the canvas.

<figure><img src="../../.gitbook/assets/image (1199).png" alt=""><figcaption><p>Marker mode enabled</p></figcaption></figure>

9.3. Sample freehand markings are shown in the image below.

<figure><img src="../../.gitbook/assets/image (1200).png" alt=""><figcaption><p>Sample markings in the report</p></figcaption></figure>

9.4. Markings can be erased using the **Clear Marker** option. Switching to another tab also results in the markings getting erased.

<figure><img src="../../.gitbook/assets/image (1203).png" alt=""><figcaption><p>Clearing markings</p></figcaption></figure>

9.5. Customize markings from Notes Settings.&#x20;

You can set the color, shape, and width of markers.

<figure><img src="../../.gitbook/assets/image (1205).png" alt=""><figcaption><p>Marker customizations</p></figcaption></figure>

In the next section, we'll look at Inforiver's [data-level commentary](comments.md) capability.
