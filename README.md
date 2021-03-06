# LINE Beacon for micro:bit

[View readme on github pages](https://pizayanz.github.io/pxt-linebeacon/)

[Japanese is here (日本語はこちら)](README_JP.md)

## Version dependency

### for micro:bit v2

This linebeacon extension conflicts with bluetooth extension, so can't be used together.

### for micro:bit v1

This linebeacon extension works with bluetooth extension.


## Usage

This package makes micro:bit to LINE Beacon.

## What's LINE Beacon

LINE beacon delivers some content to LINE App on Android/iOS device using BLE. 

Users will be able to receive contents matching the place such as visiting coupons and storefront product information from LINE from the beacon installed in the store.

[https://developers.line.me/en/docs/messaging-api/using-beacons/](https://developers.line.me/en/docs/messaging-api/using-beacons/)

## Quick Start

1. Register and get your HWID at [https://admin-official.line.me/beacon/register](https://admin-official.line.me/beacon/register)
1. Add a 'LINE Beacon start' block and copy & paste your HWID (5 bytes hex).

first compile takes few minutes.

## Sample

```blocks
input.onButtonPressed(Button.A, function () {
    basic.showIcon(IconNames.Yes)
    linebeacon.start("0f0f0f0f0f")
})
input.onButtonPressed(Button.AB, function () {
    basic.showIcon(IconNames.Yes)
    linebeacon.startWithDeviceMessage(
    "0f0f0f0f0f",
    "1a2b3c4d5e6f70809010a0b0c0"
    )
})
input.onButtonPressed(Button.B, function () {
    basic.showIcon(IconNames.No)
    linebeacon.stop()
})
basic.showIcon(IconNames.Heart)
```

## License

MIT

## Supported targets

* for PXT/microbit

<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>