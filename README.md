# googleSheetNotes

### Range properties


Get 
```js
//Range
let tableRange = tableStartCell.getDataRegion()
//values[0][0]  (empty values are returned as empty strings)
let values = tableRange.getValues()

Logger.log(tableRange.getColumn()) //2 (first column)
Logger.log(tableRange.getLastColumn()) //49 (last column)

Logger.log(tableRange.getRow()) //42 (first row)
Logger.log(tableRange.getLastRow()) //54 (last row)
```

### Search for text

```js
var finder = ss.createTextFinder(tableLabel)
var tableStartCell = finder.findNext()
```
