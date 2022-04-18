> **This is a fork of [stellar/slingshot/starsig](https://github.com/stellar/slingshot/tree/main/starsig)** (original crate [here](https://crates.io/crates/starsig)). The only difference from the upstream is that the signer does not commit to its verification key as part of the signature (i.e., the verification key will not be in the payload of the hash `c` used in the signature).

# Starsig: schnorr signatures on Ristretto

Implementation of a simple Schnorr signature protocol
implemented with [Ristretto](https://ristretto.group) and [Merlin transcripts](https://merlin.cool).

* [Specification](docs/spec.md)

## Features

* Simple message-based API.
* Flexible [transcript](https://merlin.cool)-based API.
* Single signature verification.
* Batch signature verification.
* Compatible with [Musig](../musig) API.
* Compatible with [Keytree](../keytree) key derivation API.
* VRF (aka “HMAC verifiable by a public key”) is in development.

## Authors

* [Oleg Andreev](https://github.com/oleganza)
* [Cathie Yun](https://github.com/cathieyun)
