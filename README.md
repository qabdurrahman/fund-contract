## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

-   **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
-   **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
-   **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
-   **Chisel**: Fast, utilitarian, and verbose solidity REPL.

## Documentation

https://book.getfoundry.sh/

## Usage

### Build

```shell
$ forge build
```
## Inspect
```
$ forge inspect FundMe storageLayout
```

### Test
It is used for testing
```shell
$ forge test
$ forge test -vv
$ forge script script/Interactions.s.sol:FundFundMe --rpc-url [rpcurl] --private-key [privatekey]
```
-vv specifies the visibility of logging in ----?
(do gpt for the same to understand it better)

### Format

```shell
$ forge fmt
$ forge test --fork-url $SEPOLIA_RPC_URL -vvvv
```
-vv is just for more visibility as more the v more is the visibility

### Gas Snapshots
# A file is created with the name .gas-snapshot for the gas
```shell
$ forge snapshot
```

### Anvil

```shell
$ anvil
```

### Deploy

```shell
$ forge script script/Counter.s.sol:CounterScript --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Cast

```shell
$ cast <subcommand>
```

### Help

```shell
$ forge --help
$ anvil --help
$ cast --help
```
# To add to git use git add .
