## PureCloud WebRTC SDK

[![Greenkeeper badge](https://badges.greenkeeper.io/MyPureCloud/purecloud-webrtc-sdk.svg)](https://greenkeeper.io/)

### Overview
The PureCloud WebRTC SDK is a client library for connecting to PureCloud WebRTC
services. Supported WebRTC Features:

- WebRTC SoftPhone (Authenticated Business User/Agent Telephony - inbound/outbound, etc)

Not yet supported:

- WebRTC Video
- WebRTC Screen Share
- WebRTC Screen Recording
- WebRTC Click-to-Call (Unauthenticated user SoftPhone, Telephony)

### Usage

Module import:

- `npm install --save purecloud-webrtc-sdk`

```js
const PureCloudWebrtcSdk = require('purecloud-webrtc-sdk');
const sdk = new PureCloudWebrtcSdk({
  accessToken: 'your-access-token'
});
sdk.initialize();
```

Or via global module

```html
<script src="https://sdk-cdn.mypurecloud.com/webrtc-sdk/latest/purecloud-webrtc-sdk.js"></script>
<script>
  const sdk = new window.PureCloudWebrtcSdk({
    accessToken: 'your access token'
  });
  sdk.initialize();
</script>
```

### Documentation

Documentation is in doc/documentation.md and available on the PureCloud Developer Center
at [DeveloperCenter][1]


### Contributing

This repo uses [semistandard][2] for code style, Ava for tests, and Istanbul/NYC for
code coverage.

To get started in development:
```sh
npm install
npm run watch-tests
```

Test will rebuild as source or tests change. All linting (semistandard) and tests must
pass 100%, and coverage should remain at 100%.

### Testing
Run the tests using `npm test` in the command line

[1]: https://developer.mypurecloud.com
[2]: https://github.com/Flet/semistandard
