# THIS REPO HAS BEEN ARCHIVED. THIS VERSION OF SCAMBIO IS NOT TO BE USED, PLEASE GO TO [THE OFFICIALLY SUPPORTED ONE!](https://github.com/discoin/scambio)
# Scambio

**Project Status**

[![GitHub](https://img.shields.io/github/license/cfanoulis/scambio?logo=github&style=flat-square)](https://github.com/cfanoulis/scambio/blob/master/LICENSE.md)

**Social**

[![Twitter Follow](https://img.shields.io/twitter/follow/thisiscfanoulis?label=Follow%20@thisiscfanoulis&logo=twitter&colorB=1DA1F2&style=flat-square)](https://twitter.com/thisiscfanoulis/follow)
[![Twitter Follow](https://img.shields.io/github/stars/cfanoulis/scambio?style=flat-sqaure&logo=github)](https://twitter.com/thisiscfanoulis/follow)

Scambio (which means `exchange` in Italian) is a TypeScript wrapper for Discoin

# Installation

Installation is simple. Just use:
```bash
yarn add scambio

# Or, if you'd fancy npm

npm install scambio

```

# Documentation
All the properties have TSDocs attached, so you should get documentation inside your IDE. Nevertheless, here's an example of what this wrapper can do:
```ts
import { ScambioClient } from 'scambio'
// Or, if you use JavaScript: const { ScambioClient } = require('scambio')

const client = new ScambioClient('exampleToken', 'DIC')

// Creating a transaction
const transaction = await client.createTransaction(100, 'userID', 'DTS')

// Getting a transaction by ID
const transaction2 = await client.getTransaction('transactionId')

// Getting all the unhandled transactions
const unhandledTransactions = await client.getUnhandledTransactions()

// Marking a transaction as complete
const completedTransaction = await transaction.process()
// `completedTransaction.handled` is now true
```

## API coverage
[x] Getting transactions

[x] Creating transactions

[ ] Getting currency lists


# About

## Contributing
Pull requests are issues are always welcome! Please use the issue tracker for bug requests and feature submissions

## Legal
Copyright 2019-Present ©  [Charalampos Fanoulis](https://enkiel.cloud). Distributed under the [MIT licence](LICENCE).

## Credits and honorable mentions
This project is based on the original [Discoin Wrapper](https://github.com/Discoin/nodejs-wrapper)

And of course, this project wouldn't be possible without the aid of the following amazing patrons:
- Brianna

Check out how you can support me below

## Buy me a coffee/tea/donut

Most of my projects are open-source, and they will stay so even if I run out of funds. However, should you want to fund this project, as well as my thirst for Spotify Premium, feel free to donate using the following ways:

| Method | Address | Notes |
|:------:|:-------:|:------|
|[![Pledge to me on Patreon](.github/readme-assets/patreon.jpg)](https://www.patreon.com/join/enkiel8029?)| [Pledge to me on Patreon](https://www.patreon.com/join/enkiel8029?) | Patrons get exclusive access to pre-release projects, discounts on comissions, behind-the-scenes posts and more!|
|[![Donate using PayPal](https://www.paypalobjects.com/digitalassets/c/website/marketing/na/us/logo-center/9_bdg_secured_by_pp_2line.png)](https://cfanoulis.page.link/donate-paypal) | [Donate using PayPal](https://cfanoulis.page.link/donate-paypal)
|[![Donate using bitcoin](.github/readme-assets/btc.png)](bitcoin:bc1q3e5jhh9qrk4g80ljlvu66u2dsr89v57g5madjr?message=Donation%20to%20Charalampos%27s%20OSS%20projects&time=1577294923)|`bc1q3e5jhh9qrk4g80ljlvu66u2dsr89v57g5madjr`| [Here's a premade request](bitcoin:bc1q3e5jhh9qrk4g80ljlvu66u2dsr89v57g5madjr?message=Donation%20to%20Charalampos%27s%20OSS%20projects&time=1577294923)|
|![Donate using Stellar](.github/readme-assets/stellar.png)| `cfanoulis*keybase.io`| If your wallet or network doesn't support federation, use `GCVAESPQ3OSXZQCTLJNEXD35GA5CWXPQ6FG6JVBFIDNRRJIG77OKUB4I` as the address
