# Kanswap (Rinkeby Only)

[![Tests](https://github.com/Uniswap/uniswap-interface/workflows/Tests/badge.svg)](https://github.com/Uniswap/uniswap-interface/actions?query=workflow%3ATests)
[![Styled With Prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://prettier.io/)

## Deployment

### Address

- Owner Address: 0xB5b32B39863C7c2a84d3592237e1A79798020E92
- Factory Address: 0xd5d723882d9f2d8e02506f4413e82f5b7b39f888
- WETH Address: 0xe9a31ae67302ca172c426e2cd8a1878006dff026
- Router Address: 0x11bdf0b08a714b34be1ed0b0472f054a053cbe2d

### TEST ERC20 Tokens

- KAN: [0x5c254f2481d70d1bf4f0c43cb923aa14cd62075a](https://rinkeby.etherscan.io/token/0x5c254f2481d70d1bf4f0c43cb923aa14cd62075a)
- KAN2: [0x5b6a7cfca79ee09b4f154fd1c7ed7e1f5ff796d7](https://rinkeby.etherscan.io/token/0x5b6a7cfca79ee09b4f154fd1c7ed7e1f5ff796d7)

## Accessing the Uniswap Interface

To access the Uniswap Interface, use an IPFS gateway link from the
[latest release](https://github.com/Uniswap/uniswap-interface/releases/latest),
or visit [app.uniswap.org](https://app.uniswap.org).

## Listing a token

Please see the
[@uniswap/default-token-list](https://github.com/uniswap/default-token-list)
repository.

## Development

### Install Dependencies

```bash
yarn
```

### Run

```bash
yarn start
```

### Configuring the environment (optional)

To have the interface default to a different network when a wallet is not connected:

1. Make a copy of `.env` named `.env.local`
2. Change `REACT_APP_NETWORK_ID` to `"{YOUR_NETWORK_ID}"`
3. Change `REACT_APP_NETWORK_URL` to e.g. `"https://{YOUR_NETWORK_ID}.infura.io/v3/{YOUR_INFURA_KEY}"`

Note that the interface only works on testnets where both
[Uniswap V2](https://uniswap.org/docs/v2/smart-contracts/factory/) and
[multicall](https://github.com/makerdao/multicall) are deployed.
The interface will not work on other networks.

## Contributions

**Please open all pull requests against the `master` branch.**
CI checks will run against all PRs.

## Accessing Uniswap Interface V1

The Uniswap Interface supports swapping against, and migrating or removing liquidity from Uniswap V1. However,
if you would like to use Uniswap V1, the Uniswap V1 interface for mainnet and testnets is accessible via IPFS gateways
linked from the [v1.0.0 release](https://github.com/Uniswap/uniswap-interface/releases/tag/v1.0.0).
