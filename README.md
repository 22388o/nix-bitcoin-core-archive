# nix-bitcoin-core-archive 

[nix-bitcoin](https://github.com/fort-nix/nix-bitcoin) is useful for running up-to-date `bitcoin-core`.

But sometimes, we need to run old or patched releases in a nix environment.

`nix-bitcoin-core-archive` provides Nix derivations for:
- old and outdated `bitcoin-core` releases
- development forks 

(e.g.: [`github.com/Sjors/bitcoin`](https://github.com/Sjors/bitcoin) for a SV2-patch TP)

Note: `bitcoin-wallet` and `bitcoin-qt` are not yet supported by the derivations.

## instructions

Just `cd` into the directory of the chosen `bitcoin-core` version, and then do a `nix-build`. The build artifacts will be placed at `result`. For example, if you want to run `bitcoin-core-0.21.0`:
```
$ cd bitcoin-core-0.21.0
$ nix-build
$ ls result/bin
bitcoin-cli  bitcoind  bitcoin-tx  bitcoin-util
``` 
---

# Custom Patches

 - [x] [`SV2 Patch by @Sjors`](https://github.com/Sjors/stratum) - v25.99.0
 - [x] [`SV2 + testnet4 Patch by @Sjors + @fjahr + @stratospher](https://github.com/plebhash/bitcoin) - v25.99.0
 - [x] [`MutinyNet Patch by @benthecarman`](https://github.com/benthecarman/bitcoin) - v24.99.0
 - 
---

# Bitcoin Core

 - [ ] Bitcoin Core v25.1
 - [ ] Bitcoin Core v25.0
 - [ ] Bitcoin Core v24.2
 - [ ] Bitcoin Core v24.1
 - [ ] Bitcoin Core v24.0.1
 - [ ] Bitcoin Core v23.2
 - [ ] Bitcoin Core v23.1
 - [ ] Bitcoin Core v23.0
 - [ ] Bitcoin Core v22.1
 - [x] Bitcoin Core v22.0
 - [ ] Bitcoin Core v0.21.2
 - [ ] Bitcoin Core v0.21.1
 - [x] Bitcoin Core v0.21.0
 - [ ] Bitcoin Core v0.20.2
 - [ ] Bitcoin Core v0.20.1
 - [ ] Bitcoin Core v0.20.0
 - [ ] Bitcoin Core v0.19.1
 - [ ] Bitcoin Core v0.19.0.1
 - [ ] Bitcoin Core v0.18.1
 - [ ] Bitcoin Core v0.18.0
 - [ ] Bitcoin Core v0.17.1
 - [ ] Bitcoin Core v0.17.0.1
 - [ ] Bitcoin Core v0.17.0
 - [ ] Bitcoin Core v0.16.3
 - [ ] Bitcoin Core v0.16.2
 - [ ] Bitcoin Core v0.16.1
 - [ ] Bitcoin Core v0.16.0
 - [ ] Bitcoin Core v0.15.2
 - [ ] Bitcoin Core v0.15.1
 - [ ] Bitcoin Core v0.15.0.1
 - [ ] Bitcoin Core v0.15.0
 - [ ] Bitcoin Core v0.14.3
 - [ ] Bitcoin Core v0.14.2
 - [ ] Bitcoin Core v0.14.1
 - [ ] Bitcoin Core v0.14.0
 - [ ] Bitcoin Core v0.13.2
 - [ ] Bitcoin Core v0.13.1
 - [ ] Bitcoin Core v0.13.0
 - [ ] Bitcoin Core v0.12.1
 - [ ] Bitcoin Core v0.12.0
 - [ ] Bitcoin Core v0.11.2
 - [ ] Bitcoin Core v0.11.1
 - [ ] Bitcoin Core v0.11.0

 - bitcoind -signet -signetchallenge=512102f7561d208dd9ae99bf497273e16f389bdbd6c4742ddb8e6b216e64fa2928ad8f51ae -signetblocktime=30 -rpcallowip=0.0.0.0/0
