# secure-ecdh-secret

`<secure-ecdh-secret>` A Polymer element to create a service worker subscription.

[API Docs and Demo](https://heka-house-polymer-demos.firebaseapp.com/secure-ecdh-secret)

[Source](http://github.com/hekahouse/secure-ecdh-secret/)


## Install

    bower install --save HekaHouse/secure-ecdh-secret

## Example

    <secure-ecdh-secret
      subscription-key-path="https://YOUR-FIREBASE.firebaseio.com/subscriptions/SUBSCRIPTION-ID"
      subscription="{{subscriptionKey}}">
    </secure-ecdh-secret>

## Note

Upon successful subscription the subscription key is saved to Firebase under subscription key path

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

secure-ecdh-secret depends on

[firebase-input](https://heka-house-polymer-demos.firebaseapp.com/firebase-input)

## Related
