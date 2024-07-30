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
* You can [export](../10.-exporting-reports/export.md) notes along with the report in Excel and PDF. You can also [write back](../12.-data-writeback/) to databases, shared drives, or URLs.
* Notes added in reading mode will not be saved to the base report. Report users can however export notes.
{% endhint %}

Note: With Inforiver Enterprise 2.0, there are a few changes in the notes configuration options. The updated UI/UX is shown below.

<figure><img src="../../.gitbook/assets/New UI.png" alt=""><figcaption><p>Inforiver Enterprise version 2.0</p></figcaption></figure>

## 1. Cell-level notes

a) Let's see how to add notes. Click on a cell, click 'Notes', and then 'Add new note'.

{% hint style="info" %}
To add the same note for multiple cells, Ctrl + click to select each cell, then add a note.
{% endhint %}

<figure><img src="../../.gitbook/assets/8.1.3 Notes.png" alt=""><figcaption><p>Adding a new note</p></figcaption></figure>

b) An editor opens where you can add hyperlinks and apply rich formatting. Enter a note as shown below.

<figure><img src="../../.gitbook/assets/8.1.4 Notes.png" alt=""><figcaption><p>Notes editor</p></figcaption></figure>

c) Try out the formatting options as shown below. Click 'Save'.

<figure><img src="../../.gitbook/assets/8.1.5 Notes.png" alt=""><figcaption><p>Applying rich formatting</p></figcaption></figure>

d) You can see an indicator and as you hover over it, you can see the note.

<figure><img src="../../.gitbook/assets/8.1.6 Notes.png" alt=""><figcaption><p>Notes is visible on hover</p></figcaption></figure>

e) All the notes added to the report can be seen in one place. Click  'Notes' and 'View all notes' from the dropdown. The cell-level notes can be seen in the 'All' tab,.

<figure><img src="../../.gitbook/assets/8.1.6(2) Notes.png" alt=""><figcaption><p>Cell level note in the notes panel</p></figcaption></figure>

f) You may need to enter a note that applies to multiple cells, for example, a particular marketing strategy may have contributed to the increase in sales for specific regions and quarters. You can select a series of cells and add a single note that applies to all of them.

<figure><img src="../../.gitbook/assets/3.1. Single note gif.gif" alt=""><figcaption><p>Single note for multiple cells</p></figcaption></figure>

## 2. Header-level notes

a) To add a note at the row or column header level, select the row/column. Click on the 'Notes' icon. A side panel opens providing a large screen editor.

<figure><img src="../../.gitbook/assets/8.1.7 Header notes.png" alt=""><figcaption><p>Header level notes</p></figcaption></figure>

b) Enter the note. Let's now change the color of the notes indicator. Click on a different color from the bottom of the side panel.

<figure><img src="../../.gitbook/assets/8.1.8 Header notes.png" alt=""><figcaption><p>Changing the indicator color</p></figcaption></figure>

c) You also have the option to select a custom color for the indicator. Click on the multicolored icon as highlighted in the image.

<figure><img src="../../.gitbook/assets/8.1.9 Header notes.png" alt=""><figcaption><p>Custom color for note indicator</p></figcaption></figure>

d) In addition to the formatting options available for cell-level notes, you also have numbered/bulleted lists. Click 'Save'.

<figure><img src="../../.gitbook/assets/8.1.10 Header notes.png" alt=""><figcaption><p>Adding numbered/bulleted lists</p></figcaption></figure>

e) Header-level notes are visible both in the side panel and on hover.

<figure><img src="../../.gitbook/assets/8.1.11 Header notes.png" alt=""><figcaption><p>Header-level notes</p></figcaption></figure>

f) Similarly, select a row and add a note. You can edit/delete the note using the corresponding icons on the right.

<figure><img src="../../.gitbook/assets/8.1.11(2) Header notes.png" alt=""><figcaption><p>Row category note</p></figcaption></figure>

## 3. Report-level notes

With Inforiver, you can also add notes and explanations at the report level as shown below.

a) Click on 'Notes' and then 'Report Summary'. In the 'Report Summary' side panel, enter the note.

<figure><img src="../../.gitbook/assets/Report level notes 1.png" alt=""><figcaption><p>Report level note</p></figcaption></figure>

b) On clicking 'Save', the note gets displayed in the side panel. You can edit/delete the note by clicking on the corresponding icon in the top right.

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

Notes can be added in a separate column.&#x20;

a) In the 'Notes' dropdown, turn the 'Notes column' toggle on.

<figure><img src="../../.gitbook/assets/8.1.16 Notes column.png" alt=""><figcaption><p>Adding a notes column</p></figcaption></figure>

b) A notes column gets added. Double-click on a cell and start typing in the rich text editor. You can apply formatting such as bold, italic, underline, font/background color and hyperlinks.

<figure><img src="../../.gitbook/assets/8.1.17 Notes column (1).png" alt=""><figcaption><p>Rich text formatting for notes column</p></figcaption></figure>

## 7. Hide notes

a) To hide the footnotes, turn off the footnote toggle.

b) To hide the notes column, turn off the notes column toggle.

c) To hide the cell, header, and report-level notes, turn on the 'Hide all notes' toggle. Note that by using this option, all the notes including the footnotes and notes column are hidden.&#x20;

<figure><img src="../../.gitbook/assets/8.1.15 Hide notes.png" alt=""><figcaption><p>Hiding all notes</p></figcaption></figure>

## 8. Settings

You can customize the notes indicator, position, footnote height and more.&#x20;

a) Click on 'Settings' from the 'Notes' dropdown.

<figure><img src="../../.gitbook/assets/8.1.18 Settings.png" alt=""><figcaption><p>Customization options for notes</p></figcaption></figure>

b) A dialog box opens. The default selections are shown in the below image.

<figure><img src="../../.gitbook/assets/8.1.19 Settings.png" alt=""><figcaption><p>Default settings for notes</p></figcaption></figure>

c) There are a number of indicator types such as numbered, lettered, arrow etc. Indicators can also be resized. By default, indicators are to the left of the cell. We have made changes to the default settings and the result is shown in the below image.

<figure><img src="../../.gitbook/assets/8.1.22 Settings.png" alt=""><figcaption><p>Changes made to the indicators and footnotes</p></figcaption></figure>

The notes indicator can be set at the report level (as shown above), in which case all notes in a report would have the same indicator. You can set individual indicators for each note as well.

<figure><img src="../../.gitbook/assets/image (10) (1) (1) (1).png" alt=""><figcaption><p>Notes indicator</p></figcaption></figure>

## 9. Marker mode

‘Marker Mode’ can be used to highlight important observations during presentations. Markings are temporary and can be cleared.&#x20;

a) In the 'Notes' dropdown, turn the 'Marker mode' toggle on.

<figure><img src="../../.gitbook/assets/8.1.23 Marker mode.png" alt=""><figcaption><p>Marker mode</p></figcaption></figure>

b) You can see a marker icon on the canvas.

<figure><img src="../../.gitbook/assets/8.1.24 Marker mode.png" alt=""><figcaption><p>Marker mode on</p></figcaption></figure>

c) In the below image, you can see some sample markings.

<figure><img src="../../.gitbook/assets/8.1.25 Marker mode.png" alt=""><figcaption><p>Markings added</p></figcaption></figure>

d) Markings can be erased using the ‘Clear Markings’ option. Switching to another tab also results in the markings getting erased.

<figure><img src="../../.gitbook/assets/8.1.26 Marker mode.png" alt=""><figcaption><p>Clear markings</p></figcaption></figure>

In the next section, we'll look at Inforiver's [data-level commentary](comments.md) capability.
