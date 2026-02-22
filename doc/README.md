Re-Fork is neither hard-, nor soft-fork, but Alt-Coin re-using Blockchain code with checks tweaked.
===================================================================================================
+++++++++++++++++++++  File added by bitcoin-refork (not in bitcoin-core)  ++++++++++++++++++++++++
===================================================================================================

A soft-fork results in only 1 blockchain; whereas a hard-fork creates 2 where there was 1.

Soft forks and hard forks are software / protocol upgrades to a blockchain,
that differ in compatibility and impact.

Soft Fork: A backward-compatible upgrade. where new rules are stricter than old ones.
Newer versions check for the feature, and adapt accordingly.
Nodes not upgraded can still validate new blocks, so the network remains unified. 
It does not create a new blockchain or new tokens.  
  Example: Bitcoin’s SegWit upgrade improved scalability without splitting the chain. 

Hard Fork: A non-backward-compatible change that creates a permanent split. 
Nodes must upgrade to stay on the new chain. If not, they remain on the original chain, 
resulting in two separate blockchains and two separate cryptocurrencies.  
  Example: Bitcoin Cash was created from a hard fork of Bitcoin, 
           giving existing holders of Bitcoin, an equivalent extra amount of Bitcoin Cash;
           to some this seems a repeat of the Double-Spend problem, unduely burdening it. 

Alt-Coin: A different Genesis-Block,and thus Blockchain:

Re-Fork: If a Blockchain re-uses Blockchain code (with only necessary tweaks), 
but renews Genesis-Block and Code / Genesis-Block Verification, then techincally it's 
an (Alt-Coin) Re-Fork.

===================================================================================================

Bitcoin Core
=============

Setup
---------------------
Bitcoin Core is the original Bitcoin client and it builds the backbone of the network. It downloads and, by default, stores the entire history of Bitcoin transactions, which requires several hundred gigabytes or more of disk space. Depending on the speed of your computer and network connection, the synchronization process can take anywhere from a few hours to several days or more.

To download Bitcoin Core, visit [bitcoincore.org](https://bitcoincore.org/en/download/).

Running
---------------------
The following are some helpful notes on how to run Bitcoin Core on your native platform.

### Unix

Unpack the files into a directory and run:

- `bin/bitcoin-qt` (GUI) or
- `bin/bitcoind` (headless)
- `bin/bitcoin` (wrapper command)

The `bitcoin` command supports subcommands like `bitcoin gui`, `bitcoin node`, and `bitcoin rpc` exposing different functionality. Subcommands can be listed with `bitcoin help`.

### Windows

Unpack the files into a directory, and then run bitcoin-qt.exe.

### macOS

Drag Bitcoin Core to your applications folder, and then run Bitcoin Core.

### Need Help?

* See the documentation at the [Bitcoin Wiki](https://en.bitcoin.it/wiki/Main_Page)
for help and more information.
* Ask for help on [Bitcoin StackExchange](https://bitcoin.stackexchange.com).
* Ask for help on #bitcoin on Libera Chat. If you don't have an IRC client, you can use [web.libera.chat](https://web.libera.chat/#bitcoin).
* Ask for help on the [BitcoinTalk](https://bitcointalk.org/) forums, in the [Technical Support board](https://bitcointalk.org/index.php?board=4.0).

Building
---------------------
The following are developer notes on how to build Bitcoin Core on your native platform. They are not complete guides, but include notes on the necessary libraries, compile flags, etc.

- [Dependencies](dependencies.md)
- [macOS Build Notes](build-osx.md)
- [Unix Build Notes](build-unix.md)
- [Windows Build Notes](build-windows-msvc.md)
- [FreeBSD Build Notes](build-freebsd.md)
- [OpenBSD Build Notes](build-openbsd.md)
- [NetBSD Build Notes](build-netbsd.md)

Development
---------------------
The Bitcoin repo's [root README](/README.md) contains relevant information on the development process and automated testing.

- [Developer Notes](developer-notes.md)
- [Productivity Notes](productivity.md)
- [Release Process](release-process.md)
- [Source Code Documentation (External Link)](https://doxygen.bitcoincore.org/)
- [Translation Process](translation_process.md)
- [Translation Strings Policy](translation_strings_policy.md)
- [JSON-RPC Interface](JSON-RPC-interface.md)
- [Unauthenticated REST Interface](REST-interface.md)
- [BIPS](bips.md)
- [Dnsseed Policy](dnsseed-policy.md)
- [Benchmarking](benchmarking.md)
- [Internal Design Docs](design/)

### Resources
* Discuss on the [BitcoinTalk](https://bitcointalk.org/) forums, in the [Development & Technical Discussion board](https://bitcointalk.org/index.php?board=6.0).
* Discuss project-specific development on #bitcoin-core-dev on Libera Chat. If you don't have an IRC client, you can use [web.libera.chat](https://web.libera.chat/#bitcoin-core-dev).

### Miscellaneous
- [Assets Attribution](assets-attribution.md)
- [bitcoin.conf Configuration File](bitcoin-conf.md)
- [CJDNS Support](cjdns.md)
- [Files](files.md)
- [Fuzz-testing](fuzzing.md)
- [I2P Support](i2p.md)
- [Init Scripts (systemd/upstart/openrc)](init.md)
- [Managing Wallets](managing-wallets.md)
- [Multisig Tutorial](multisig-tutorial.md)
- [Offline Signing Tutorial](offline-signing-tutorial.md)
- [P2P bad ports definition and list](p2p-bad-ports.md)
- [PSBT support](psbt.md)
- [Reduce Memory](reduce-memory.md)
- [Reduce Traffic](reduce-traffic.md)
- [Tor Support](tor.md)
- [Transaction Relay Policy](policy/README.md)
- [ZMQ](zmq.md)

License
---------------------
Distributed under the [MIT software license](/COPYING).
