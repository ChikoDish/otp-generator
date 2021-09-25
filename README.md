# otp-generator
Generate OTP with specific digits and seeds

[![Build Status][travis-ci-img]][travis-ci-url] 
[![npm version][npm-version-img]][npm-version-url]
[![Test Coverage][coveralls-image]][coveralls-url]
[![js-standard-style][js-standard-style-img]][js-standard-style-url] 

[![NPM](https://nodei.co/npm/otp-generators.png?downloadRank=true&downloads=true)](https://www.npmjs.com/package/otp-generators/)

## Index
* [Install](#install)
* [Usage](#usage)

## Install

```bash
npm i otp-generators
```

## Usage

```js
var newOTP = require('otp-generators)

newOTP.generate(6, { alphabets: false, upperCase: false, specialChars: false });

```
### generate(length, options)

**Arguments**

* `length` - length of password. Optional if `options` is optional. default length is 6.
* `options` - optional
  - `digits` - Default: `true` true value includes digits in OTP 
  - `alphabets` - Default: `true` true value includes alphabets in OTP
  - `upperCase` - Default: `true` true value includes uppercase alphabets in OTP
  - `specialChar` - Default: `true` true value includes special Characters in OTP

## License
[MIT][license-url]
