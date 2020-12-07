# LINE Beacon for micro:bit

[Japanese is here (日本語はこちら)](README_JP.md)

## Version dependency

2018.11 This package does not work well on latest JavaScript Blocks Editor, now.

Please use old one.
https://makecode.microbit.org/v0

## Usage

This package makes micro:bit to LINE Beacon.

## What's LINE Beacon

LINE beacon delivers some content to LINE App on Android/iOS device using BLE. 

Users will be able to receive contents matching the place such as visiting coupons and storefront product information from LINE from the beacon installed in the store.

https://developers.line.me/en/docs/messaging-api/using-beacons/

## Quick Start

1. Register and get your HWID at https://admin-official.line.me/beacon/register
1. Add a 'LINE Beacon start' block and copy & paste your HWID (5 bytes hex).

first compile takes few minutes.

## Sample

![Sample](./docs/LINEBeaconSample.png "Sample")

## License

MIT

## Supported targets

* for PXT/microbit

<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>