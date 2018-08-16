Dashcore Library
================

[![NPM Package](https://img.shields.io/npm/v/@botcoin-core/botcore-lib.svg?style=flat-square)](https://www.npmjs.org/package/@botcoin-core/botcore-lib)
[![Build Status](https://img.shields.io/travis/botcoin-core/botcore-lib.svg?branch=master&style=flat-square)](https://travis-ci.org/botcoin-core/botcore-lib)
[![Coverage Status](https://img.shields.io/coveralls/botcoin-core/botcore-lib.svg?style=flat-square)](https://coveralls.io/github/botcoin-core/botcore-lib?branch=master)

A pure and powerful JavaScript Botcoin library.

## Principles

Botcoin is a powerful new peer-to-peer platform for the next generation of financial technology. The decentralized nature of the Botcoin network allows for highly resilient Botcoin infrastructure, and the developer community needs reliable, open-source tools to implement Botcoin apps and services.

## Get Started
### NodeJS
```
npm install @botcoin-core/botcore-lib
```

### Browser

See the section below to generate your own bundle, or download the pre-generated [minified file](dist/botcore-lib.min.js)


## Docs

* [Addresses](docs/address.md)
* [Block](docs/block.md)
* [Crypto](docs/crypto.md)
* [Encoding](docs/encoding.md)
* [Hierarchically-derived Private and Public Keys](docs/hierarchical.md)
* [Networks](docs/networks.md)
* [PrivateKey](docs/privatekey.md)
* [PublicKey](docs/publickey.md)
* [Script](docs/script.md)
* [Transaction](docs/transaction.md)
* [Using Different Units](docs/unit.md)
* [Unspent Output](docs/unspentoutput.md)
* [URI](docs/uri.md)
* [Governance Object / Proposal](docs/govobject/govobject.md)

## Examples

Some examples can be found [here](docs/examples.md), below is a list of direct links for some of them.


* [Generate a random address](docs/examples.md#generate-a-random-address)
* [Generate an address from a SHA256 hash](docs/examples.md#generate-a-address-from-a-sha256-hash)
* [Import an address via WIF](docs/examples.md#import-an-address-via-wif)
* [Create a Transaction](docs/examples.md#create-a-transaction)
* [Sign a Botcoin message](docs/examples.md#sign-a-bitcoin-message)
* [Verify a Botcoin message](docs/examples.md#verify-a-bitcoin-message)
* [Create an OP RETURN transaction](docs/examples.md#create-an-op-return-transaction)
* [Create a 2-of-3 multisig P2SH address](docs/examples.md#create-a-2-of-3-multisig-p2sh-address)
* [Spend from a 2-of-2 multisig P2SH address](docs/examples.md#spend-from-a-2-of-2-multisig-p2sh-address)

## Modules

Some functionality is implemented as a module that can be installed separately:

* [Payment Protocol Support](https://github.com/botcoin-core/botcore-payment-protocol)
* [Peer to Peer Networking](https://github.com/botcoin-core/botcore-p2p)
* [Botcoin Core JSON-RPC](https://github.com/botcoin-core/dashd-rpc)
* [Payment Channels](https://github.com/botcoin-core/botcore-channel)
* [Mnemonics](https://github.com/botcoin-core/botcore-mnemonic)
* [Elliptical Curve Integrated Encryption Scheme](https://github.com/botcoin-core/bitcore-ecies-botcoin)
* [Signed Messages](https://github.com/botcoin-core/bitcore-message-botcoin)

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://github.com/botcoin-core/botcore-lib/blob/master/CONTRIBUTING.md) file.

## Building the Browser Bundle

To build a botcore-lib full bundle for the browser:

```sh
npm run build
```

This will generate files named `botcore-lib.js` and `botcore-lib.min.js` in the `dist/` folder.

## Usage on Browser

```
<script src='./dist/botcore-lib.min.js' type="text/javascript"></script>
<script>
  const PrivateKey = botcore.PrivateKey;
  const privateKey = new PrivateKey();
  const address = privateKey.toAddress().toString();
</script>
```

## Development & Tests

```sh
git clone https://github.com/botcoin-core/botcore-lib
cd botcore-lib
npm install
```

Run all the tests:

```sh
npm test
```

You can also run just the Node.js tests with `npm run test:node`, just the browser tests with `npm run test:browser`
or run a test coverage report with `npm run coverage`.

## License

Code released under [the MIT license](LICENSE).

Copyright 2013-2017 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.  
Copyright 2016-2017 The Botcoin Foundation, Inc.  
Copyright 2017-2018 Botcoin Core Group, Inc.  
