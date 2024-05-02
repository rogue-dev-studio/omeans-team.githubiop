---
title: "How To Show Timezone"
description: Examples Script To Show Timezone Like +0700.
author: aris_h
date: 2024-04-03 17:54:57 +0700
categories: [Tutorial]
tags: [timezone, javascript]
---


### How To Show Timezone

```js
    const date = new Date();
    const timezoneOffset = date.getTimezoneOffset();
    const timezoneOffsetHours = Math.abs(timezoneOffset / 60);
    const timezoneOffsetMinutes = Math.abs(timezoneOffset % 60);
    const timezoneOffsetSign = timezoneOffset > 0? "-" : "+";
    const timezoneOffsetFormatted = timezoneOffsetSign + timezoneOffsetHours.toString().padStart(2, "0") + timezoneOffsetMinutes.toString().padStart(2, "0");

    console.log(timezoneOffsetFormatted); // Output: "+07:00"
```

Hasilnya akan menampilkan +07:00