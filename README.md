# secure-ecdh-secret

`<secure-ecdh-secret>` A polymer element providing ECDH secret derivation in Chrome and Firefox.

[API Docs and Demo](https://heka-house-polymer-demos.firebaseapp.com/secure-ecdh-secret)

[Source](http://github.com/hekahouse/secure-ecdh-secret/)


## Install

    bower install --save HekaHouse/secure-ecdh-secret

## Example

    <secure-ecdh-secret
      client-auth-secret="{{FCM AUTH SECRET}}"
      receiver-key="{{FCM P256 KEY}}"
      shared-secret="{{sharedSecret}}">
    </secure-ecdh-secret>

The following properties must be populated with base64 strings prior to trigger secret creation:

clientAuthSecret (provided with service worker subscription to FCM/GCM)

receiverKey (provided with service worker subscription to FCM/GCM)

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

secure-ecdh-secret depends on

[secure-utils](http://github.com/hekahouse/secure-utils/)

includes embedded browser version of [Elliptic](https://github.com/indutny/elliptic)

Elliptic is used because Chrome doesn't support importing public ECDH keys using Web Crypto API

If this support is provided in the future Elliptic should be replaced with Web Crypto key import

## Related

[secure-fcm-crypto](http://github.com/hekahouse/secure-fcm-crypto/)

[service-worker-subscription](http://github.com/hekahouse/service-worker-subscription/)
