# [Fa Fa Fa](https://www.youtube.com/watch?v=N6xoFhkthls)

This is a small Eth2 dev testnet, with permissioned validator access, to debug P2P bugs on, and have dev fun!

## Validating

If you like to run a validator, ping @protolambda,
 give your Goerli testnet Ath1 address and ask for deposit tokens.

## Configuration

See repository files for config files for each client.

- Spec version: `v0.12.2`
- Genesis Time: `1596710871` (`2020-08-06T10:47:51Z`)
- Genesis Fork Version: `0x00fafafa`
- Fork Digest: `0xa3778fcd`
- Initial State Root: `0xa2b1679d94e730dc19bc3e5645d760b2fdffed6036ce2aa875117e766de45764`
- Genesis Block Root: `0xf197f88e0b2c9d9dd7ea2122c07d1eb0939cbe424117de50c8d851d3564e8305`
- Deposit Contract: [`0xc15Bf10aAfd93360AC77Ce3bfE5272f854017dF7`](https://goerli.etherscan.io/address/0x38c750cFFb382cDD3644C40A39540a9b4b46b0cf) (_Note_ this is a modified deposit contract with access control features. See [`beta-1`](../README.md#attacker-validators) rules for more details on registering validators)
- Deposit Contract Deploy Block Hash: `0x76e947b593081b2fa2621053782bf15f587bb6ae9ab48c43b5314957ff924f9d`
- Deposit Contract Deploy Block Number: `3174222`
- `MIN_GENESIS_TIME`: `1578009600`
- `MIN_GENESIS_ACTIVE_VALIDATOR_COUNT`: `520`
- `GENESIS_DELAY`: `900`
- Bootnode ENR(s):
  - `enr:-Ku4QDEawcgXZkMQzasM55ki8dgcscN_iEiePQYdUh3JZQT2JEyZogsU9AfibVSaSxkW81pDlAqrqs0YoTEjGhZUX4YBh2F0dG5ldHOIAAAAAAAAAACEZXRoMpCgyVg2APr6-v__________gmlkgnY0gmlwhCLqwe6Jc2VjcDI1NmsxoQK8R63gDqak_oNJ6e4PkICnAwBiLVBhWE800oNHYRnRI4N1ZHCCIyg`
- Chain Explorers: None
- Status Dashboard: [fafafa.eth2.wtf](https://fafafa.eth2.wtf)
