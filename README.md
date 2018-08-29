[![Build Status](https://travis-ci.org/gergelyke/express-security.txt.svg?branch=master)](https://travis-ci.org/gergelyke/express-security.txt)

[![NPM](https://nodei.co/npm/express-security.txt.png?compact=true)](https://nodei.co/npm/express-security.txt/) [![Greenkeeper badge](https://badges.greenkeeper.io/gergelyke/express-security.txt.svg)](https://greenkeeper.io/)

## node-security.txt

### Usage

#### Install with:

```bash
npm i express-security.txt -S
```

#### Add to your app with:

```javascript
const express = require('express')
const securityTxt = require('express-security.txt')

const app = express()

app.get('/security.txt', securityTxt({
  // your security address
  contact: [
    'mailto:email@example.com',
    'tel:+123456789'
   ],
  // your pgp key
  encryption: 'https://example.com/security.gpg',
  // if you have a hall of fame for securty resourcers, include link here
  acknowledgements: 'https://acknowledgements.example.com'
}))
```
