---
title: 'buffer'
attributions:
  - 'Microsoft Developer Network: [Windows Internet Explorer JavaScript reference Article](http://msdn.microsoft.com/en-us/library/ie/yek4tbz0%28v=vs.94%29.aspx)'
compatibility:
  feature: buffer
  topic: javascript
readiness: 'Ready to Use'
summary: 'Read-only. Gets the ArrayBuffer that is referenced by this array.'
tags:
  - JS_Basic
uri: javascript/Float64Array/buffer

---
## Summary

Read-only. Gets the ArrayBuffer that is referenced by this array.

## Syntax

    var arrayBuffer = float64Array.buffer;

## Examples

The following example shows how to get the ArrayBuffer of the array.

``` js
var req = new XMLHttpRequest();
     req.open('GET', "http://www.example.com");
     req.responseType = "arraybuffer";
     req.send();

     req.onreadystatechange = function () {
         if (req.readyState === 4) {
             var buffer = req.response;
             var dataView = new DataView(buffer);
             var floatArr = new Float64Array(buffer.byteLength / 8);
             alert(floatArr.buffer.byteLength);
         }
     }
```

