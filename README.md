# msx-hlsx
Media Station X hls.js player with audio tracks and subtitles.

That's a mod of the original hls.js player that allows to choose audio and subtitle tracks like html5x does.

This plugin was tested with a stream with multiple quality options and subtitle tracks.

# Usage

`https://slonopot.github.io/msx-hlsx/hlsx.html?url={URL}`

For example:

```
{
    "type": "pages",
    "headline": "HLSX Plugin Test",
    "template": {
        "type": "separate",
        "layout": "0,0,2,4",
        "icon": "msx-white-soft:extension",
        "color": "msx-glass",
        "playerLabel": "whatever",
        "action": "video:plugin:https://slonopot.github.io/msx-hlsx/hlsx.html?url=https://mtoczko.github.io/hls-test-streams/test-gap/playlist.m3u8",
        "properties": {
            "resume:position": "102",
            "button:content:icon": "{context:contentIcon}",
            "button:content:action": "{context:contentAction}",
        }
    },
    "items": [
        {
            "title": "Test",
            "titleFooter": "Whatever",
            "contentIcon": "settings",
            "contentAction": "panel:request:player:options"
        }
    ]
}
```

# Shoutouts

[Media Station X](https://msx.benzac.de/info/)

[The original plugin](https://msx.benzac.de/wiki/index.php?title=HTML5X_Plugin)