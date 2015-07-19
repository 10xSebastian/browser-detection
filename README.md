BrowserDetection
=================

Javascript library for detecting the browser (navigator name) and version.
If you want to enable some functionalities of your Web-App just for some browser/version combinations use `BrowserDetection.match`.

How to use
-----------------
```
  var browserSupported = BrowserDetection.match([
    {
      name: "Chrome",
      version: 29
    },{
      name: "Opera",
      name: 12,
    }
  ]);

  if(browserSupported) {
    initYourFeature();
  }

  BrowserDetection.match({name: "Chrome"}) // true
  BrowserDetection.match({name: "Chrome", version: 29}) // true
  BrowserDetection.match([{name: "Chrome", version: 29},{name: "Firefox", version: 10}]) // true

  BrowserDetection.name() // "Chrome"
  BrowserDetection.version() // "29.0.1547.57"
  BrowserDetection.major() // 29
```

Browsers supported/tested
-----------------
- Chrome <= 29
- Firefox <= 23
- Opera <= 12
- Safari <= 6
- Internet Explorer <= 11

Release notes
-----------------
* 2.0.0 Change API: 'isSupported' becomes 'match'
* 1.0.3 Patch to fix messed up version management: 'isSupported' is the interface again
* 1.0.1 Support Internet Explorer 11
