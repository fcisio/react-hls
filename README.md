# React HLS Player

## Introduction

`react-hls-player` is a simple hls/rtmp live stream player.
It uses [hls.js](https://github.com/video-dev/hls.js) to play your hls live stream if your browser supports `html 5 video` and `MediaSource Extension`.

## Example

```javascript
<ReactHlsPlayer
    url='https://bitdash-a.akamaihd.net/content/sintel/hls/playlist.m3u8'
    autoplay={false}
    controls={true}
    width={500}
    height={375}
/>
```


## Props
Prop | Description
------------ | -------------
url [ `String`, `required` ] | The hls url that you want to play
autoplay [ `Boolean` ] | Autoplay when component is ready. Defaults to `false`
controls [ `Boolean` ] | Whether or not to show the playback controls. Defaults to `false`
width [ `Number` ] | Video width
height [ `Number` ] | Video height
hlsConfig [ `Object` ] | `hls.js` config , you can see all config [here](https://github.com/video-dev/hls.js/blob/master/docs/API.md#fine-tuning)
videoProps [ `Object` ] | All video tag attributes supported. You can check [all attributes here](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/video)
poster [ `String` ] | Poster image for video player [as described here](https://www.w3schools.com/tags/att_video_poster.asp)
ref [ `React Ref` ] | Pass in your own ref to interact with the video player directly. This will override the default ref.
