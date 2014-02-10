paste.js
=====

paste.js is an interface to read from clipboard data in different browsers. Currenttly only tested under: 

* IE 11 (Windows 7)
* Chrome 32 (Windows 7 / OSX)
* Firefox 26 (Windows 7 / OSX)
* Opera 12.15 (OSX) (text only)

usage
-----

```
// jQuery needed
paste = $.paste();
paste.on('pasteImage', function (ev, data){
  console.log("dataURL: " + data.dataURL)
});
paste.on('pasteText', function (ev, data){
  console.log("text: " + data.text)
});
paste.focus(); // it's actually a hidden div element

// ... when you don't need it anymore
paste.remove();
```

more
-----

see [this example](http://puffant.github.io/paste.js/)
