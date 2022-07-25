# Fornaxswap SDK

[//]: # ([![code style: prettier]&#40;https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square&#41;]&#40;https://github.com/prettier/prettier&#41;)

[//]: # ([![Actions Status]&#40;https://github.com/Uniswap/uniswap-sdk/workflows/CI/badge.svg&#41;]&#40;https://github.com/Uniswap/uniswap-sdk&#41;)

[//]: # ([![npm version]&#40;https://img.shields.io/npm/v/@uniswap/sdk/latest.svg&#41;]&#40;https://www.npmjs.com/package/@uniswap/sdk/v/latest&#41;)

[//]: # ([![npm bundle size &#40;scoped version&#41;]&#40;https://img.shields.io/bundlephobia/minzip/@uniswap/sdk/latest.svg&#41;]&#40;https://bundlephobia.com/result?p=@uniswap/sdk@latest&#41;)

[//]: # (In-depth documentation on this SDK is available at [uniswap.org]&#40;https://uniswap.org/docs/v2/SDK/getting-started/&#41;.)

## Address Modifications

When deploying a new instance in Fornax, you need to modify the address in the following files:

WFRX: `./src/entities/token.ts`
Factory: `./src/constants.ts`

## Running tests

To run the tests, follow these steps. You must have at least node v10 and [yarn](https://yarnpkg.com/) installed.

First clone the repository:

```sh
git clone https://github.com/FornaxCoin/fornaxswap-sdk.git
```

Move into the fornaxswap-sdk working directory

```sh
cd fornaxswap-sdk/
```

Install dependencies

```sh
yarn install
```

Run tests

```sh
yarn test
```

You should see output like the following:

```sh
yarn run v1.22.4
$ tsdx test
 PASS  test/constants.test.ts
 PASS  test/pair.test.ts
 PASS  test/fraction.test.ts
 PASS  test/miscellaneous.test.ts
 PASS  test/entities.test.ts
 PASS  test/trade.test.ts

Test Suites: 1 skipped, 6 passed, 6 of 7 total
Tests:       3 skipped, 82 passed, 85 total
Snapshots:   0 total
Time:        5.091s
Ran all test suites.
✨  Done in 6.61s.
```
