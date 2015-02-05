# NetEase Cloud SDK for JavaScript in Node.js

Since there's no official NetEase Cloud SDK for JavaScript, I stole
[aws-sdk-js](https://github.com/aws/aws-sdk-js) and made this crappy port.

## Installing in Node.js

```sh
npm install nec-sdk
```

## Usage and Getting Started

This SDK is very similar to AWS SDK.

You can find a getting started guide for AWS SDK at:

http://docs.aws.amazon.com/AWSJavaScriptSDK/guide/

## Supported Services

Currently only NOS (Netease Object Storage) is supported. And the API
definitions is just a copy of AWS S3, with metadata and default config
modified.

## License

The license of AWS SDK JS is
[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).
And this SDK is distributed under the same licence.

It seems the license asks me to list all modified files, they are:

* .gitignore
* apis/metadata.json
* lib/aws.js
* lib/signers/request_signer.js
* NOTICE.txt
* package.json
* README.md

And I add a few files of my own, they are:

* apis/nos-2015-12-05.min.json
* lib/signers/nos.js

I'm not quite familiar with the license. Please let me know if I did something
wrong. Thank you!

## Change Log

* 2015-02-05 v1.0.1  NOS: Allow slashes in object key.
* 2015-02-04 v1.0.0  Add NOS API.
