# react-native-get-mp3-duration

> Computes the duration of an mp3 buffer in react native

[![NPM](https://img.shields.io/npm/v/get-mp3-duration.svg)](https://www.npmjs.com/package/get-mp3-duration) [![Build Status](https://travis-ci.com/transitive-bullshit/get-mp3-duration.svg?branch=master)](https://travis-ci.com/transitive-bullshit/get-mp3-duration) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save get-mp3-duration
# or
yarn add get-mp3-duration
```

## Usage

```js
import getMP3Duration from 'get-mp3-duration';
import {FileSystem} from 'react-native-file-access'; // or another lib that read the file into base64

const bufferStr = await FileSystem.readFile('fixtures/vbr.mp3', 'base64')
const duration = await getMP3Duration(bufferStr)

console.log(duration, 'ms') => 285727 ms
```

## Related

- [mp3-duration](https://github.com/ddsol/mp3-duration) this package is a fork of mp3-duration to add browser support.
- [vmsg](https://github.com/Kagami/vmsg) is an optimized mp3 recorder for the web which ports the lame mp3 encoder to wasm.

## License

MIT © [Travis Fischer](https://github.com/transitive-bullshit)

Support my OSS work by <a href="https://twitter.com/transitive_bs">following me on twitter <img src="https://storage.googleapis.com/saasify-assets/twitter-logo.svg" alt="twitter" height="24px" align="center"></a>
