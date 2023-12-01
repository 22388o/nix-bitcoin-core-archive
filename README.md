# nix-bitcoin-core-archive 

[nix-bitcoin](https://github.com/fort-nix/nix-bitcoin) is useful for running up-to-date `bitcoin-core`.

But sometimes, we need to run old or patched releases in a nix environment.

`nix-bitcoin-core-archive` provides Nix derivations for:
- old and outdated `bitcoin-core` releases
- development forks (e.g.: [`github.com/Fi3/bitcoin`](https://github.com/Fi3/bitcoin) for a SV2-patch TP)

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

 - [ ] Bitcoin Core 25.1
 - [ ] Bitcoin Core 25.0
 - [ ] Bitcoin Core 24.2
 - [ ] Bitcoin Core 24.1
 - [ ] Bitcoin Core 24.0.1
 - [ ] Bitcoin Core 23.2
 - [ ] Bitcoin Core 23.1
 - [ ] Bitcoin Core 23.0
 - [ ] Bitcoin Core 22.1
 - [ ] Bitcoin Core 22.0
 - [ ] Bitcoin Core 0.21.2
 - [ ] Bitcoin Core 0.21.1
 - [x] Bitcoin Core 0.21.0
 - [ ] Bitcoin Core 0.20.2
 - [ ] Bitcoin Core 0.20.1
 - [ ] Bitcoin Core 0.20.0
 - [ ] Bitcoin Core 0.19.1
 - [ ] Bitcoin Core 0.19.0.1
 - [ ] Bitcoin Core 0.18.1
 - [ ] Bitcoin Core 0.18.0
 - [ ] Bitcoin Core 0.17.1
 - [ ] Bitcoin Core 0.17.0.1
 - [ ] Bitcoin Core 0.17.0
 - [ ] Bitcoin Core 0.16.3
 - [ ] Bitcoin Core 0.16.2
 - [ ] Bitcoin Core 0.16.1
 - [ ] Bitcoin Core 0.16.0
 - [ ] Bitcoin Core 0.15.2
 - [ ] Bitcoin Core 0.15.1
 - [ ] Bitcoin Core 0.15.0.1
 - [ ] Bitcoin Core 0.15.0
 - [ ] Bitcoin Core 0.14.3
 - [ ] Bitcoin Core 0.14.2
 - [ ] Bitcoin Core 0.14.1
 - [ ] Bitcoin Core 0.14.0
 - [ ] Bitcoin Core 0.13.2
 - [ ] Bitcoin Core 0.13.1
 - [ ] Bitcoin Core 0.13.0
 - [ ] Bitcoin Core 0.12.1
 - [ ] Bitcoin Core 0.12.0
 - [ ] Bitcoin Core 0.11.2
 - [ ] Bitcoin Core 0.11.1
 - [ ] Bitcoin Core 0.11.0
