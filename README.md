<h1 align=center><a href="https://cofix.io"><code>CoFiX</code></a></h1>

<p align=center> <i>A computable financial transaction model</i> </p>
<p align=center> <i>The Future of On-Chain Market Making is Here 🤑 📈📉💰</i> </p>


<p align="center">
  <a href="https://github.com/Computable-Finance/CoFiX/actions?query=workflow%3ACoFiX">
    <img src="https://github.com/Computable-Finance/CoFiX/workflows/CoFiX/badge.svg" />
  </a>
  <a href="https://travis-ci.org/Computable-Finance/CoFiX">
    <img src="https://travis-ci.org/Computable-Finance/CoFiX.svg?branch=master" />
  </a>
  <a href="https://coveralls.io/github/Computable-Finance/CoFiX?branch=master">
    <img src="https://coveralls.io/repos/github/Computable-Finance/CoFiX/badge.svg?branch=master" />
  </a>
  <a href="https://www.gnu.org/licenses/gpl-3.0">
    <img src="https://img.shields.io/badge/License-GPLv3-green.svg" />
  </a>
</p>

<!-- # [CoFiX](https://cofix.io/)

*A computable financial transaction model*

![CoFiX](https://github.com/Computable-Finance/CoFiX/workflows/CoFiX/badge.svg)
[![Build Status](https://travis-ci.org/Computable-Finance/CoFiX.svg?branch=master)](https://travis-ci.org/Computable-Finance/CoFiX)
[![Coverage Status](https://coveralls.io/repos/github/Computable-Finance/CoFiX/badge.svg?branch=master)](https://coveralls.io/github/Computable-Finance/CoFiX?branch=master) -->

## Whitepaper

**[https://cofix.io/doc/CoFiX_White_Paper.pdf](https://cofix.io/doc/CoFiX_White_Paper.pdf)**

## Documentation

**[https://docs.cofix.io/](https://docs.cofix.io/)**

## Usage

### Run test

```shell
npm install

npm run test
```

### Compile

Run `truffle compile`, get build results in `build/contracts` folder, including `ABI` json files.

or

Use `npx oz compile` to adopt `@openzeppelin/cli` toolchain.

### Deploy

Deploy with `truffle` and you will get a contract deployement summary on contract addresses.

```shell
truffle migrate --network ropsten
```

You may need to `activate()` the price oracle through `CoFiXController` contract manually and set kTable with the help of [scripts/setKTable.js](scripts/setKTable.js).

### Scripts

There are several scripts used to invoke with the protocol in [`scripts/`](scripts) folder. Simplely run `truffle exec scripts/SPECIFIC_SCRIPT.JS` with flags to execute. Here are some [examples](docs/change_controller.md).

### Generate ABI

```shell
npm run genabi
```

## Mainnet

### Beta-V0.6

|       Contract       |                  Address                   |
| :------------------: | :----------------------------------------: |
| USDT | 0xdAC17F958D2ee523a2206206994597C13D831ec7 |
| HBTC | 0x0316EB71485b0Ab14103307bf65a021042c6d380 |
| NEST | 0x04abEdA201850aC0124161F037Efd70c74ddC74C |
| WETH | 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 |
| NestPriceOracle | 0x7722891Ee45aD38AE05bDA8349bA4CF23cFd270F |
| CoFiXController | 0xC16E5eECc0948604eb326296c71311aC8D9BC786 |
| CoFiXFactory | 0xD5a19E1ADb5592921dcC42E48623d75c4C91e405 |
| CoFiXKTable | 0x75E360Be6248Bd46030C6818624a09403EF5eC21 |
| CoFiXRouter | 0x2878469c466638E8c0878bB86898073CA6C91b45 |

## Ropsten Testnet

### Beta-V0.1

|       Contract       |                  Address                   |
| :------------------: | :----------------------------------------: |
|     CoFiXRouter     | 0x07F4385F741f873423dedE6C2645698FcB287683 |
|    CoFiXFactory     | 0x869EfF8B605E0B5Ba3E8B9F81C199B2BBB3e34Df |
|      USDT Token      | 0xB5852d2cC06cd394f52C9edEbF0f1d59aD4A0615 |
|         WETH         | 0x1A2c206FcE664440c0b953df0C976B1208F411Eb |
| NEST3PriceOracleMock | 0x9dE1109708926C90117DAFB23F13176Bb6d878E0 |

### Beta-V0.2

|       Contract       |                  Address                   |
| :------------------: | :----------------------------------------: |
|      CoFiXRouter     | 0xEa19497F26eeF50A68CD4502410471f41C23B563 |
|     CoFiXFactory     | 0x2F3DC9488C8cea30c2DcA6Bb78aD15d1E37206B7 |
|      USDT Token      | 0x83a1e68dA9Fa81B3a54dDc49Fbb2c13cf4f7239d |
|         WETH         | 0xd44b717a5d54a9520b411d0f297eD69ef81Af10e |
|   CoFiXController    | 0x01B5fF069b49d2dA08cCBce9D8506d59472Ea868 |
| NEST3PriceOracleMock | 0xf137Dd7C6f091494597e0907D234E486128Bc937 |

### Beta-V0.3

|       Contract       |                  Address                   |
| :------------------: | :----------------------------------------: |
| USDT | 0xDc9E7381678EfA251E403F8F9fafcBdbf91a5C6C |
| HBTC | 0x081B96b53f887ef4543649CED7fD7A5a872bDd29 |
| WETH9 | 0xcfcF136eEc1C4A03BC2F684090844bF67168bF90 |
| NEST3PriceOracleMock | 0x33EB7860427220684D6d69E0CE1914FfBFaC56B1 |
| CoFiXController | 0x6D631e101BC36A6f51fB875059347B1D4830BdBB |
| CoFiXFactory | 0xD9aB2Ca67641f11e808d32ffc5741a3A0d44E05c |
| CoFiXRouter | 0x442A92e41EEFA4567a75d27773A9A64e8d3A6880 |

### Beta-V0.4

|       Contract       |                  Address                   |
| :------------------: | :----------------------------------------: |
| USDT | 0xD52d3bfCA0d39E4bD5378e0BBa8AD245C3F58C17 |
| HBTC | 0x9aA0AF152cf141740f19D335b5ddE1F0E51008A7 |
| NEST | 0xB9746A8572DB5C27597fE88B86B6520599Bf62d4 |
| WETH9 | 0xB3d7C7993BE7bEec23D005552224B2dAf18Bd85E |
| NEST3PriceOracleMock | 0x2183B4bC72c299FDDFf27D4bDBc635bbc8cA5e44 |
| CoFiXController | 0xf2Fe41C81C60698E2abE1B8cb7BB56C5570e3C55 |
| CoFiXFactory | 0xde33584665ea098748897B1292150c003b855df6 |
| CoFiXKTable | 0xDB69107004694428aab5E6F196dcdd588F52B745 |
| CoFiXRouter | 0x2cC5b038bd296779A3a50430179cB8C6a02B9D13 |

### Beta-V0.7

|       Contract       |                  Address                   |
| :------------------: | :----------------------------------------: |
| USDT | 0x200506568C2980B4943B5EaA8713A5740eb2c98A |
| HBTC | 0xA674f71ce49CE7F298aea2F23D918d114965eb40 |
| NEST | 0xD287Bc43eCD3D892204aA3792165fe8728636E29 |
| WETH | 0x59b8881812Ac484Ab78b8fc7c10b2543e079a6C3 |
| CoFiToken | 0xA1B66D21DC42cCCDe55F06f381CbcecD422Ef4d4 |
| CoFiStakingRewards | 0x8bEEfdc9Ba635E2451d275Ca1b9AfEe3C13D65d7 |
| NestPriceOracle | 0x70B9b6F0e1E4073403cF7143b45a862fe73af3B9 |
| CoFiXController | 0x636520329ee488Cb99552Ab225267668608b179a |
| CoFiXFactory | 0xf56E0C6E9D3233b99FA439710147E52b9ef26F60 |
| CoFiXKTable | 0xe609B978635c7Bb8D22Ffc4Ec7f7a16615a3b1cA |
| CoFiXRouter | 0x30f1c72CfcF96c4de2e279fa256567F8ADbEf888 |
| CoFiXVaultForLP | 0x4F6544aF9Ea4107b52D4563F16c2A660D1E7EB41 |

### Beta-V0.8

|       Contract       |                  Address                   |
| :------------------: | :----------------------------------------: |
| USDT | 0x200506568C2980B4943B5EaA8713A5740eb2c98A |
| HBTC | 0xA674f71ce49CE7F298aea2F23D918d114965eb40 |
| NEST | 0xD287Bc43eCD3D892204aA3792165fe8728636E29 |
| WETH | 0x59b8881812Ac484Ab78b8fc7c10b2543e079a6C3 |
| NestPriceOracle | 0x70B9b6F0e1E4073403cF7143b45a862fe73af3B9 |
| CoFiXKTable | 0xe609B978635c7Bb8D22Ffc4Ec7f7a16615a3b1cA |
| CoFiToken | 0x93c9753e638d242d1ca9EDa04962b0dEbd775D99 |
| CNodeToken | 0x5F0025E59514c3E8c7aabbca08D46Ff01DFe483B |
| CoFiXFactory | 0x87067A940C2c0c5B878FeB2c92bBddcc46Cebb01 |
| CoFiXRouter | 0xfF3951f94c38812a76a9eb717A9af47391652A32 |
| CoFiXController | 0x15192BeCf3bDA4915fc1282282a5cF384cA653c6 |
| CoFiXVaultForLP | 0x283D7D9Ce67F26DdefC9bbcE14B08c267cbf7A2f |
| CoFiXVaultForTrader | 0x5C8AA2C4355252E5D461aDC95f733eC2e45c63c8 |
| CoFiXVaultForCNode | 0xAdDB1f88D9c742ACaD1a1A6fd46Baad294618aae |
| CoFiStakingRewards | 0xfDEa9b00220C4901834dc1d9f467D8Cb52300B41 |

## Kovan Testnet

### Beta-V0.5

|       Contract       |                  Address                   |
| :------------------: | :----------------------------------------: |
| USDT | 0x04716BaA169f6E5BAFe92E4643C2f18480ba46D3 |
| HBTC | 0xcae23767DF5BbEBD0d64402a7d3d82776f97bE46 |
| NEST | 0x08cFf00044dECe1D817F3D30A7cc8aef43A284De |
| WETH | 0x6A04aF9c9793D9eE1a27eB7A343f940282a0AB9e |
| NestPriceOracle | 0x93Afa4ff16874Cf9D4f29da4973be277f53607Af |
| CoFiXController | 0xf71141F66e15740DB5d59E4c31ee0D84d6584452 |
| CoFiXFactory | 0x9984dCe65387d9AE8a495452F72dF0A0D4F85d2c |
| CoFiXKTable | 0x0441e7e4C1ecd73a068F0696Cf4cB10Ea69dD74A |
| CoFiXRouter | 0xB5852d2cC06cd394f52C9edEbF0f1d59aD4A0615 |

## Test Flow

check [`test/CoFiX.test.js`](test/CoFiX.test.js) for details.
