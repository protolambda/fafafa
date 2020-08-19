# [Fa Fa Fa](https://www.youtube.com/watch?v=N6xoFhkthls)

This is a small Eth2 dev testnet, with permissioned validator access, to debug P2P bugs on, and have dev fun!

## Validating

**IMPORTANT: The deposit contract is permissioned with a token system.**

If you like to run a validator, ping @protolambda,
 give your Goerli testnet Eth1 address and ask for deposit tokens.

## Configuration

See repository files for config files for each client.

- Spec version: `v0.12.2`
- Genesis Time: `1597835294` (`2020-08-19T11:08:14Z`)
- Genesis Fork Version: `0x01fafafa`
- Fork Digest: node: `0x340cec0f`, bootnode: `0xcf5bb1f3` 
- Initial State Root: `0x96826f5730654bba59663e2eda3168432980624e722de3c435cea1fc67dbb68c`
- Genesis Block Root: `0x1ef0e7663461571447a56bfefdd76f83da0b2d6db1250fed0baa9e6fe74c90e3`
- Deposit Contract: [`0x1dd8A52b4Eb0BaA6bB6aF57c36AACe8727BdfccB`](https://goerli.etherscan.io/address/0x1dd8A52b4Eb0BaA6bB6aF57c36AACe8727BdfccB) (_Note_ this is a modified deposit contract with access control features.)
- Deposit Contract Deploy Block Hash: `0xc0986743deb660aa0cff7a21fc0aeeaf16c5143d1f3dda5a3dadd0c40aac549f`
- Deposit Contract Deploy Block Number: `3251570`
- `MIN_GENESIS_TIME`: `1578009600`
- `MIN_GENESIS_ACTIVE_VALIDATOR_COUNT`: `512`
- `GENESIS_DELAY`: `900`
- Bootnode ENR(s):
  - `enr:-Ku4QDEawcgXZkMQzasM55ki8dgcscN_iEiePQYdUh3JZQT2JEyZogsU9AfibVSaSxkW81pDlAqrqs0YoTEjGhZUX4YBh2F0dG5ldHOIAAAAAAAAAACEZXRoMpCgyVg2APr6-v__________gmlkgnY0gmlwhCLqwe6Jc2VjcDI1NmsxoQK8R63gDqak_oNJ6e4PkICnAwBiLVBhWE800oNHYRnRI4N1ZHCCIyg`
- Chain Explorers: None
- Status Dashboard: [fafafa.eth2.wtf](https://fafafa.eth2.wtf)

**Nimbus**: you need this PR to be merged into your branch for the config to work:
 https://github.com/status-im/nim-beacon-chain/pull/1453

## Eth2stats

Something like this, replace client type, display name, beacon API and metrics port numbers:
```shell script
eth2stats-client run \
--eth2stats.node-name="Nimbus heya" \ 
--data.folder=/data \
--eth2stats.addr=grpc.fafafa.eth2.wtf:8080 \
--eth2stats.tls=false \
--beacon.type=nimbus \
--beacon.addr=http://localhost:4000 \ 
--beacon.metrics-addr=http://localhost:8080/metrics
```

Available as docker image: `alethio/eth2stats-client:latest`
