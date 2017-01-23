# Node Ocr

## Pre Installation
需先安裝[node-tessract](https://github.com/desmondmorris/node-tesseract)

## Example

```javascript
var tesseract = require('node-tesseract')

// Recognize text of any language in any format
tesseract.process(__dirname + '\\test.png', (err, text) => {
    if (err) {
        console.error(err)
    } else {
        console.log(text)
    }
})
```
