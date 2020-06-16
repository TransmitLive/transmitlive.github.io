---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

### JWPlayer Plugin

Released Versions

| Version | Url | JWPlayer Support |  |
| v1 |**minified**<br>https://code.transmit.live/v1/transmit-live-jwplayer-plugin.min.js<br><br> **full**<br>https://code.transmit.live/v1/transmit-live-jwplayer-plugin.js| 8+ | [Live Demo](https://code.transmit.live/demo/index.html){:target="_blank"} |

TransmitLive's JWPLayer plugin supports SSAI watermarks for enhanced ad delivery and metrics.

Below is an example of how to enable the plugin for your JWPlayer:

```js
jwplayer('my-player').setup({
  playlist: [{
    file: myVideo,
  }],
  plugins: {
    'https://code.transmit.live/v1/transmit-live-jwplayer-plugin.min.js': {
      debug: true,
    }
  },
});
```

Plugin Options

| Option | Description |
| --- | ----------- |
| debug | show debug output in browser console |

Currently JWPlayer version 8+ is supported.
