## React Column Resizer

Place in between `td` tags to add resizing functionality. Works with touch and mouse events. 

Currently only supports resizing between columns. 

Flaws: The resizer needs to be wide enough to grab and you have to put filler `<td/>`'s in rows you don't use the resizer.

### Props

`number minWidth` - The minimum width for the columns (in pixels)

`string className`- Any classes you want to add (inline style will be disabled if this is set)

### Usage: 

```
<table>
    <tbody>
    
        <tr>
            <td>Header 1</td>
            
            <ColumnResizer/>
            
            <td>Header 2</td>
            
            <ColumnResizer/>
            
            <td>Header 3</td>
        </tr>
        
        <tr>
            <td>Cell (0, 0)</td>
            
            <td/>
            
            <td>Cell (0, 1)</td>
            
            <td/>
            
            <td>Cell(0, 2)</td>
        </tr>
        
    </tbody>
</table>
```