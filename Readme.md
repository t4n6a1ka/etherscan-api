# Etherscan API

[![npm](https://img.shields.io/npm/dt/etherscan-api.svg)](https://www.npmjs.com/package/etherscan-api)<<<<<<< patch-5
=======
 <<<<<<< patch-4
 >>>>>>> master
[![license](https://img.shields.io/github/license/sebs/etherscan-api.svg)](https://github.com/sebs/etherscan-api/blob/master/LICENSE.md)
[![GitHub tag](https://img.shields.io/github/tag/sebs/etherscan-api.svg)](https://github.com/sebs/etherscan-api)
[![Travis](https://img.shields.io/travis/sebs/etherscan-api.svg)](https://travis-ci.org/sebs/etherscan-api)
[![GitHub issues](https://img.shields.io/github/issues/sebs/etherscan-api.svg)](https://github.com/sebs/etherscan-api/issues)
 <<<<<<< patch-5
=======
=======
[![license](https://img.shields.io/github/license/#/etherscan-api.svg)](https://github.com/t4n6a1ka/etherscan-api/blob/master/LICENSE.md)
[![GitHub tag](https://img.shields.io/github/tag/#/etherscan-api.svg)](https://github.com/t4n6a1ka/etherscan-api)
[![Travis](https://img.shields.io/travis/t4n6a1ka/etherscan-api.svg)](https://travis-ci.org/t4n6a1ka/etherscan-api)
[![GitHub issues](https://img.shields.io/github/issues/#/etherscan-api.svg)](https://github.com/t4n6a1ka/etherscan-api/issues)
 >>>>>>> master
 >>>>>>> master

A way to access the [etherscan.io api](https://etherscan.io/apis) using promises. Fetch a diverse set of information about the blockchain.

Mainnet


```javascript
var api = require('etherscan-api').init('YourApiKey');
var balance = api.account.balance('0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae');
balance.then(function(balanceData){
  console.log(balanceData);
});
```
## Example in the wild

* [Polymer3 based example](https://github.com/hiherto-elements/test-app)

## For testnet usage

Supported:

* morden
* ropsten
* rinkeby

Latest

```javascript
// apikey, network, timeout
var api = require('etherscan-api').init('YourApiKey','rinkeby'. '3000');
```


## Install

 ```bash
 npm install etherscan-api --save
 ```


## API Documentation

 <<<<<<< patch-5
[Full Api Docs](https://sebs.github.io/etherscan-api/)
=======
 <<<<<<< patch-4
[Full Api Docs](https://sebs.github.io/etherscan-api/)
=======
[Full Api Docs](https://t4n6a1ka.github.io/etherscan-api/)
 >>>>>>> master
 >>>>>>> master


## Development workflow

* npm test  - runs tests
  * npm run posttest - starts the linter
* npm run lint - preconfigured linter
* npm run docs - generates the apidocs
* npm run bundle - builds a new bundle
* npm run preversion - Steps before we create a new Tag
  * lint
  * changelog
* npm run pages - pushes generated apidocs to the server
* postversion - after generating a new version, push the tag to the server
* npm run changelog - generates a changelog and pushes it
