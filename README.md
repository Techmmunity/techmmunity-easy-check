# Techmmunity - check

[![npm](https://img.shields.io/npm/v/@techmmunity/easy-check.svg?color=2ba097)](https://www.npmjs.com/package/@techmmunity/easy-check) <space> [![Coverage Status](https://coveralls.io/repos/github/Techmmunity/easy-check/badge.svg?branch=master)](https://coveralls.io/github/Techmmunity/easy-check?branch=master) <space> [![Tests](https://github.com/Techmmunity/easy-check/workflows/tests/badge.svg)]() <space> [![Downloads](https://img.shields.io/npm/dw/@techmmunity/easy-check.svg)](https://www.npmjs.com/package/@techmmunity/easy-check)

check is a light-weigth library to check things that a lot of projects needs to check, like **email**, **username**, **phone**, and many more validations.

## Install

With Yarn:

```sh
yarn add @techmmunity/easy-check
```

With NPM:

```sh
npm i @techmmunity/easy-check
```

## Usage

With TypeScript:

```ts
import { check } from "@techmmunity/easy-check";

if (check.isEmail("example@email.com")) {
  console.log("Yes, it's an email!");
}
```

With JavaScript:

```js
const { check } = require("@techmmunity/easy-check");

if (check.isEmail("example@email.com")) {
  console.log("Yes, it's an email!");
}
```

## Tips && Tricks

### 1 - You can change the import to be less verbose, like this:

```ts
import { check: ck } from "@techmmunity/easy-check";

if (ck.isEmail("example@email.com")) {
  console.log("Yes, it's an email!");
}
```

## Methods

You can find more information about the methods in the comments of the methods declaration.

| Method              | How To Use                                                     |
| ------------------- | -------------------------------------------------------------- |
| `isEmail`           | `check.isEmail("example@email.com")`                           |
| `isEmoji`           | `check.isEmoji("😂")`                                          |
| `hasEmojis`         | `check.hasEmojis("Yes, there is emojis here 😂")`              |
| `isHerokuApiKey`    | `check.isHerokuApiKey("625628d3-8a45-466e-a55e-ead5c6886887")` |
| `isHexColor`        | `check.isHexColor("#000")`                                     |
| `hasHtmlTags`       | `check.hasHtmlTags("Foo <b>Bar</b>")`                          |
| `isIpv4`            | `check.isIpv4("192.168.1.1")`                                  |
| `isIpv4WithMask`    | `check.isIpv4WithMask("192.168.1.1/24")`                       |
| `isStrongPassword`  | `check.isStrongPassword("$t0ngP@ssw0rD")`                      |
| `isBrazillianPhone` | `check.isBrazillianPhone("2199999999")`                        |
| `isSimpleUsername`  | `check.isSimpleUsername("user-name")`                          |
