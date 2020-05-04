# Textformatter Table
This is a Textformatter for the [ProcessWire CMS](https://www.processwire.com). It will take text between TABLE-- --TABLE and surround it with table-tags or div-tags with a table-class. Newlines will become rows. Columns will generated with |. If the first line has no columns, it will be a caption.

```
TABLE---Sample Table
Head1|Head2|Head3
Cell1|Cell2|Cell3---TABLE
```
will become
```html
<table>
    <caption>Sample Table</caption>
    <tr><td>Head1</td><td>Head2</td><td>Head3</td></tr>
    <tr><td>Cell1</td><td>Cell2</td><td>Cell3</td></tr>
</table>
```
and
```
TABLE---Sample Table
TH---Head1|Head2|Head3
Cell1|Cell2|Cell3---TABLE
```
will become
```html
<table>
    <caption>Sample Table</caption>
    <tr><th>Head1</th><th>Head2</th><th>Head3</th></tr>
    <tr><td>Cell1</td><td>Cell2</td><td>Cell3</td></tr>
</table>
```