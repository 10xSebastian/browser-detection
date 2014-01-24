BrowserDetection [![Build Status](https://travis-ci.org/spape/browser-detection.png)](https://travis-ci.org/spape/browser-detection)
=================

Javascript library for detecting the browser (navigator name) and version.

How to use
-----------------
```
  BrowserDetection.name() // "Chrome"
  BrowserDetection.version() // "29.0.1547.57"
  BrowserDetection.major() // 29
  BrowserDetection.isSupported({name: "Chrome"}) // true
  BrowserDetection.isSupported({name: "Chrome", version: 29}) // true
  BrowserDetection.isSupported([{name: "Chrome", version: 29},{name: "Firefox", version: 10}]) // true
```

Currently supported browsers
-----------------
- Chrome <= 29
- Firefox <= 23
- Opera <= 12
- Safari <= 6
- Internet Explorer <= 11

Release notes
-----------------
* 1.0.1 Support Internet Explorer 11