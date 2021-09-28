# etherscan-client-typescript
[![Build Status](https://travis-ci.org/Ethercast/etherscan-client.svg?branch=master)](https://travis-ci.org/Ethercast/etherscan-client)
[![codecov](https://codecov.io/gh/Ethercast/etherscan-client/branch/master/graph/badge.svg)](https://codecov.io/gh/Ethercast/etherscan-client)
[![NPM version][npm-svg]][npm]

   [npm]: https://www.npmjs.com/package/etherscan-client-typescript
   [npm-svg]: https://img.shields.io/npm/v/etherscan-client-typescript.svg?style=flat

TypeScript client for the Etherscan API

## Install
`npm i --save etherscan-client-typescript`

## Usage

```typescript
import EtherscanClient from 'etherscan-client-typescript';

async function printAbi() {
  const client = new EtherscanClient({ apiKey: 'my-key', apiUrl: 'https://api.etherscan.io/api' });
  const abi = await client.getAbi(SOME_CONTRACT_ADDRESS);
  console.log(abi);
}

```
