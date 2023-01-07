# HTML table 

## Basic Table
* HTML tables allow web developers to arrange data into rows and columns.
* A table consists of rows, columns, and cells, much like a spreadsheet. A row is a horizontal line of information. A column is a vertical line of information. A cell is the intersection of a row and a column and usually contains data
* To create a table on a webpage, start with the `<table>` and `</table>` tags and then add table rows and table data within those tags. 

```html
<table>

</table>
```
* A table in HTML consists of table cells inside rows and columns. Each table cell is defined by a `<td>` and a `</td>` tag. Everything between `<td>` and `</td>` are the content of the table cell.
* Each table row starts with a `<tr>` and ends with a `</tr>` tag. You can have as many rows as you like in a table; just make sure that the number of cells are the same in each row.

```html
<table>
  <tr>
    <td>Discrimination</td>
    <td>การแบ่งแยก</td>
  </tr>
  <tr>
    <td>Obligation</td>
    <td>ภาระ</td>
  </tr>
</table>
```

## Table headers
* Table headers define what kind of information contained in that columns (or sometime row). We create table header using the `<th>` tag

```html
<table>
    <tr>
        <th>English</th>
        <th>Thai</th>
    </tr>
    <tr>
        <td>Discrimination</td>
        <td>การแบ่งแยก</td>
    </tr>
    <tr>
        <td>Obligation</td>
        <td>ภาระ</td>
    </tr>
</table>
```

## Table Captions
* A table caption is descriptive text that serves as a title or identifies the table’s purpose. 
* The table caption text appears above a table, spans its length, and is center-aligned by default. 
* Define a table caption with a starting `<caption>` tag and an ending `</caption>` tag. When using a table caption, insert it after the starting `<table>` tag.
* A table can have only one caption
```html
<table>
    <caption> ท่องศัพท์ </caption>
    <tr>
        <th>English</th>
        <th>Thai</th>
    </tr>
    <tr>
        <td>Discrimination</td>
        <td>การแบ่งแยก</td>
    </tr>
    <tr>
        <td>Obligation</td>
        <td>ภาระ</td>
    </tr>
</table>
```
## Table Element Attributes
* You can use two primary attributes within a table:  colspan, and rowspan.
* If you need to span text or other content across two or more columns, use the
colspan attribute. 
* Likewise, if you need to span content across two or more rows, use the rowspan
attribute.
```html
<table>
      <caption>
        ท่องศัพท์
      </caption>
      <tr>
        <th>English</th>
        <th>Thai</th>
      </tr>
      <tr>
        <td rowspan="2">Discrimination</td>
        <td>การแบ่งแยก</td>
      </tr>
      <tr>
        <td>การเลือกปฏิบัติ</td>
      </tr>
      <tr>
        <td>Obligation</td>
        <td>ภาระ</td>
      </tr>
    </table>
<table>
```

```html
<table>
  <tbody><tr>
    <th>Month</th>
    <th>Day</th>
    <th>Year</th>
  </tr>
  <tr>
    <td colspan="3">January</td>
  </tr>
  <tr>
    <td>1</td>
    <td colspan="2">2022</td>
  </tr>
  <tr>
    <td colspan="3">February</td>
  </tr>
  <tr>
    <td>14</td>
    <td colspan="2">2022</td>
  </tr>
</tbody></table>
```