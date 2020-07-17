---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

### JWPlayer Plugin

TransmitLive's JWPLayer plugin supports SSAI watermarks for enhanced ad delivery and metrics.

Released Versions


| Version | Type | Url | JWPlayer Support |  |
|---|---|---|---| -- |
| v1.1.2 | [Plugin](#Plugin) | https://code.transmit.live/jwplayer/transmit-live-jwplayer-plugin.min.js| 8+ | [Live Demo](https://code.transmit.live/demo/index.html) |
| v1.1.2 | [Embed](#Embed) | https://code.transmit.live/jwplayer/transmit-live-jwplayer-embed.min.js| 8+ | [Live Demo](https://code.transmit.live/demo/jw-embed.html) |


There are two variants of the plugin.


## Plugin

**Plugin** is used to configure the plugin when calling the jwplayer setup function.
Below is an example of how to enable the plugin for your JWPlayer:

```js
jwplayer('my-player').setup({
  playlist: [{
    file: myVideo,
  }],
  plugins: {
    'https://code.transmit.live/jwplayer/transmit-live-jwplayer-plugin.min.js': {},
  },
});
```

Plugin Options

| Option | Description | Type |
| --- | ----------- | --- |
| debug | show debug output in browser console | boolean |
| hook | user provided function on page for plugin to send events | function |

## Embed
**Embed** is used alongside a content specific embed tag.

The script tag must follow directly after the jwplayer embed script tag as shown below:

```html
    <div class="player-container">
      <script src="https://cdn.jwplayer.com/players/WIAp1Zxz-0sbpeY4x.js"></script>
      <script src="https://code.transmit.live/jwplayer/transmit-live-jwplayer-embed.min.js"></script>
    </div>
```

Embed HTML Attribute Options

| Option | Description | Type |
| --- | ----------- | --- |
| data-debug | show debug output in browser console | tag attr |
| data-hook-ns | namespace for user provided function | tag attr |
|  data-hook-fn | function on page for plugin to send events | tag attr |

Currently JWPlayer version 8+ is supported.
