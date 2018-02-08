# Video2Image
## jQuery plugin for viewing/playing/stoping a webcam with image capture

###### This plugin may not work in all browsers

This plugin is used with jQuery which can be downloaded at:

 - https://jquery.com/

**selector** should be a `<canvas>` element you have added to the page.

`<canvas id="photocanvas" width="320" height="240"></canvas>`

### Initialize
`$("#photocanvas").video2image();`

### Initialize with options
```
$(selector).video2image({
  width : 320,
  height : 240,
  autoplay : true,
  onsuccess : function () {},
  onerror: function () {}
});
```

### Find out if your browser supports this

Returns true or false

`var isSupported = $(selector).video2image('isSupported');`

### To get a PNG DataURL from the canvas

Returns an image/png in base64

`var dataurl = $(selector).video2image('capture');`   

### To Stop the video
`$(selector).video2image('stop');`

### To start/restart the video
`$(selector).video2image('start');`
