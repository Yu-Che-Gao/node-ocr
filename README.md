# Node Ocr

## Pre Installation
需先安裝[tessract](https://github.com/tesseract-ocr/tesseract)

## Example

var tesseract = require('node-tesseract')

// Recognize text of any language in any format
tesseract.process(__dirname + '\\test.png', (err, text) => {
    if (err) {
        console.error(err)
    } else {
        console.log(text)
    }
})
