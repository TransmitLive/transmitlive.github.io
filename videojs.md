---
layout: page
title: Video.js Plugin
category: doc
---

### Video.js Plugin

TransmitLive's Video.js plugin supports SSAI watermarks for enhanced ad delivery and metrics.

Released Versions


| Version | Url | Video.js Support ||
|---|---|---| -- |
| v1.3.1 | https://code.transmit.live/videojs/transmit-live-videojs-plugin.min.js| 7+ |[Live Demo](https://code.transmit.live/demo/videojs.html) |

## Setup

There are two ways to set up the plugin for videojs.

Include the TransmitLive plugin script tag and use the `data-setup` attribute on the video tag. For more information refer to the [Video.js Documenation](https://docs.videojs.com/tutorial-setup.html#automatic-setup)

```html
<video id="my-video" muted class="video-js" controls preload="auto" width="800" height="450" data-setup='{"plugins":{"transmitLive":{}}}'>

<script src="https://vjs.zencdn.net/7.8.2/video.js"></script>
<script src="https://code.transmit.live/videojs/transmit-live-videojs-plugin.js"></script>
```

Include the TransmitLive plugin script tag and manually configure the player using javascript. For more information refer to the [Video.js Documenation](https://docs.videojs.com/tutorial-setup.html#manual-setup)

```html
  <script src="https://vjs.zencdn.net/7.8.2/video.js"></script>
  <script src="https://code.transmit.live/videojs/transmit-live-videojs-plugin.js"></script>
  <script>
    videojs('my-video', {
      plugins: {
        transmitLive: {}
      }
    });
  </script>
});
```

Plugin Options

| Option | Description | Type |
| --- | ----------- | --- |
| debug | show debug output in browser console via Video.js | boolean |
| hook | user provided function on page for plugin to send events | function |


<br>
<br>
<br>
