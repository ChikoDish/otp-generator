# otp-generator
Generate OTP with specific digits and seeds

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

// For numeric OTP
newOTP.generate(6, { alphabets: false, upperCase: false, specialChars: false });

// For alphanumeric OTP
newOTP.generate(6, { alphabets: true, upperCase: false, specialChars: false });

// For alphanumeric with upperCase
newOTP.generate(6, { alphabets: true, upperCase: true, specialChars: false });

// For alphanumeric with special characters 
newOTP.generate(6, { alphabets: true, upperCase: true, specialChars: true });

```
### generate(length, options)

**Arguments**

* `length` - length of password. Optional if `options` is optional. default length is 6.
* `options` - optional
  - `digits` - Default: `true` true value includes digits in OTP 
  - `alphabets` - Default: `true` true value includes alphabets in OTP
  - `upperCase` - Default: `true` true value includes uppercase alphabets in OTP
  - `specialChar` - Default: `true` true value includes special Characters in OTP

