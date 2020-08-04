# twilio-video-ios-capacitor


Capacitor plugin for make video calls using [Twilio Video](https://www.twilio.com/video) platform on iOS.  

Since the current implementation of Ionic/PWA apps on iOS run on top of WKWebView and Apple does not support WebRTC on WKWebView, the only way to work with Twilio Video on this platform is to build it natively.

> This plugin is currently under development.  
> Forked from [twilio-ios-capacitor](https://github.com/MCanhisares/twilio-ios-capacitor).

## Installation

* `npm i agodin3z/twilio-video-ios-capacitor`

## Usage

This plugin uses version 3.6 of the Twilio Video iOS Library and uses version 2.1.1 of Capacitor

```ts
import { TwilioVideoIos } from 'twilio-video-ios-capacitor';
import { Plugins } from '@capacitor/core';
const { TwilioVideoIos } = Plugins

TwilioVideoIos.joinRoom({ roomName: roomName, accessToken: accessToken})
```

## Api

| Method                                               | Default | Type                      | Description                 |
| ---------------------------------------------------- | ------- | ------------------------- | --------------------------- |
| joinRoom(options: { roomName: string, accessToken: string }) |         | `Promise<void>` | Used to join a room with the provided accessToken |
