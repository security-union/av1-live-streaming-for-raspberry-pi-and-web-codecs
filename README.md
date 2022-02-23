# Fearless AV1 live streaming for Raspberry PI and Chrome's WebCodecs

## Goals
Use the latest, greatest open source technology to live stream using a Raspberry PI.

## AV1 Streaming
AOMedia Video 1 (AV1) is an open, royalty-free video coding format initially designed for video transmissions over the Internet. It was developed as a successor to VP9 by the Alliance for Open Media (AOMedia),

## WebCodecs
Modern web technologies provide ample ways to work with video. Media Stream API, Media Recording API, Media Source API, and WebRTC API add up to a rich tool set for recording, transferring, and playing video streams. While solving certain high-level tasks, these APIs don't let web programmers work with individual components of a video stream such as frames and unmuxed chunks of encoded video or audio. To get low-level access to these basic components, developers have been using WebAssembly to bring video and audio codecs into the browser. But given that modern browsers already ship with a variety of codecs (which are often accelerated by hardware), repackaging them as WebAssembly seems like a waste of human and computer resources.

WebCodecs API eliminates this inefficiency by giving programmers a way to use media components that are already present in the browser. 

Specifically:

1. Video and audio decoders
2. Video and audio encoders
3. Raw video frames
4. Image decoders
5. The WebCodecs API is useful for web applications that require full control over the way media content is processed, such as video editors, video conferencing, video streaming, etc.


## Tech Stack

### Raspberry PI App (video-streaming)
1. Camera recorder: nokhwa https://crates.io/crates/nokhwa
2. AV1 encoder: rav1e https://crates.io/crates/rav1e
3. WebSocket server: warp https://crates.io/crates/warp

### UI (web-ui)
1. UI Framework: React https://reactjs.org/
2. Web AV1 decoder: WebCodecs https://web.dev/webcodecs/
3. WebSockets: react-use-websocket https://www.npmjs.com/package/react-use-websocket



## 👤 Contributors ✨

<table>
<tr>
<td align="center"><a href="https://github.com/darioalessandro"><img src="https://avatars0.githubusercontent.com/u/1176339?s=400&v=4" width="100" alt=""/><br /><sub><b>Dario</b></sub></a></td>
<td align="center"><a href="https://github.com/griffobeid"><img src="https://avatars1.githubusercontent.com/u/12220672?s=400&u=639c5cafe1c504ee9c68ad3a5e09d1b2c186462c&v=4" width="100" alt=""/><br /><sub><b>Griffin Obeid</b></sub></a></td>    
</tr>
</table>

## Show your support

Give a ⭐️ if this project helped you!