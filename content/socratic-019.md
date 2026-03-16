+++
title = "Socratic Seminar 19"
date = 2026-03-19
+++

Housekeeping
------------

- This meetup is generously sponsored by Presidio Bitcoin!
- Questions are encouraged, including basic ones!
- Socratic Seminars are held under the [Chatham House Rule](https://www.chathamhouse.org/about-us/chatham-house-rule): share the information you receive, but do not reveal the identity of who said it.
- For the privacy of other attendees, please refrain from taking photographs of other people without their permission.
- Socratic seminars are best when the moderator can let the conversation flow, so try to keep things concrete and focused.
- The reading list covers February 20th, 2026 to March 19th, 2026.

News
----
- [How Institutions and Businesses are Using Lightning](https://blog.bitfinex.com/education/how-institutions-and-businesses-are-using-lightning)
- [Cake Wallet Launches Bitcoin Lightning Network Support With Full Self-Custody and Privacy Defaults](https://bitcoinmagazine.com/business/cake-wallet-launches-bitcoin-lightning-network-support-with-full-self-custody-and-privacy-defaults)
- [Blockstream’s Jade Hardware Wallet Adds Lightning Network Support, Enabling Instant Bitcoin Payments From Cold Storage](https://bitcoinmagazine.com/news/blockstream-jade-wallet-lightning-network)

bLIPs & BOLTs
-------------
- [bolt11: add new test vector high-S signature with 'n' field defined](https://github.com/lightning/bolts/pull/1298)
- [Add details for post-anchor `dust_limit_satoshis`](https://github.com/lightning/bolts/pull/1301)
- [BOLT 12: add test vector for invalid bech32 padding](https://github.com/lightning/bolts/pull/1312)
- [BOLT 12: clarify that offer_amount must be greater than zero](https://github.com/lightning/bolts/pull/1316)
- [bolt02: clarify tx_init_rbf must ensure conflict with all prior attempts](https://github.com/lightning/bolts/pull/1322)

Noteworthy PRs
--------------

### [Core Lightning](https://github.com/ElementsProject/lightning)
- [Configuration option to specify "fronting nodes" for routehints/blinded paths.](https://github.com/ElementsProject/lightning/pull/8490)
- [crates: improved json codec decoding performance](https://github.com/ElementsProject/lightning/pull/8718)
- [Add `channel_id` Filter to `listpeerchannels`](https://github.com/ElementsProject/lightning/pull/8766)
- [renepay: refactor and bugfixes](https://github.com/ElementsProject/lightning/pull/8798)
- [currencyrate: new rust plugin to provide the `currencyconvert` API](https://github.com/ElementsProject/lightning/pull/8842)

### [Eclair](https://github.com/ACINQ/eclair)
- [Select `channel_type` for automatic channel creation](https://github.com/ACINQ/eclair/pull/3250)
- [Don't automatically use `scid_alias` for public channels](https://github.com/ACINQ/eclair/pull/3255)
- [Add `ChannelFundingCreated` event](https://github.com/ACINQ/eclair/pull/3256)
- [Plugin validation of interactive transactions](https://github.com/ACINQ/eclair/pull/3258)
- [Make auto-refresh relay fees from configuration optional](https://github.com/ACINQ/eclair/pull/3260)

### [LDK](https://github.com/lightningdevkit/rust-lightning)
- [[Custom Transactions] Add `TxBuilder::get_available_balances`](https://github.com/lightningdevkit/rust-lightning/pull/4026)
- [prefactor: Allow multiple htlcs in/out in forwarding events for trampoline](https://github.com/lightningdevkit/rust-lightning/pull/4304)
- [Add PaginatedKVStore traits upstreamed from ldk-server](https://github.com/lightningdevkit/rust-lightning/pull/4347)
- [lightning-block-sync: switch to bitreq, drop chunked_transfer](https://github.com/lightningdevkit/rust-lightning/pull/4350)
- [Support payments for less than the total MPP value](https://github.com/lightningdevkit/rust-lightning/pull/4373)
- [Split `DiscardFunding` from `SpliceFailed` event](https://github.com/lightningdevkit/rust-lightning/pull/4388)
- [Use HTLC CLTV instead of onion CLTV values for payment claim timer](https://github.com/lightningdevkit/rust-lightning/pull/4402)
- [Contribute to splice as acceptor](https://github.com/lightningdevkit/rust-lightning/pull/4416)
- [Avoid sending stfu for quiescent splice action while pending splice](https://github.com/lightningdevkit/rust-lightning/pull/4426)
- [Merge initial and retry stfu send paths](https://github.com/lightningdevkit/rust-lightning/pull/4432)
- [Check that funder covers the fee spike buffer multiple after a splice](https://github.com/lightningdevkit/rust-lightning/pull/4433)
- [Fix spurious `debug_assert` in UTXO gossip dedup check](https://github.com/lightningdevkit/rust-lightning/pull/4466)
- [Set max channel dust limit to 10,000 sats for all zero-fee-htlc-tx chans](https://github.com/lightningdevkit/rust-lightning/pull/4484)

### [LND](https://github.com/lightningnetwork/lnd)
- [feature: start to set the require bit for channel_type](https://github.com/lightningnetwork/lnd/pull/9637)
- [input: update taproot scripts to add an option for the miniscript compat versions from latest spec](https://github.com/lightningnetwork/lnd/pull/9639)
- [Onion message forwarding](https://github.com/lightningnetwork/lnd/pull/10089)
- [Add `AuxHtlcValidator`](https://github.com/lightningnetwork/lnd/pull/10434)
- [payments: kv-to-sql migration (tests + wiring)](https://github.com/lightningnetwork/lnd/pull/10485)
- [improve speed of retrieval of payments](https://github.com/lightningnetwork/lnd/pull/10535)
- [rpc: add channel updates to SubscribeChannelEvents](https://github.com/lightningnetwork/lnd/pull/10543)
- [switchrpc: improve SendOnion error handling](https://github.com/lightningnetwork/lnd/pull/10545)
- [[g175] graph/db: add gossip-version plumbing for core graph APIs](https://github.com/lightningnetwork/lnd/pull/10572)
- [invoices/sql_store: replace catch-all FilterInvoices with targeted index-friendly queries](https://github.com/lightningnetwork/lnd/pull/10601)
- [payments: SQL backend implementation series](https://github.com/lightningnetwork/lnd/pull/10604)
- [Update getdebuginfo rpc](https://github.com/lightningnetwork/lnd/pull/10613)
- [invoices/sql: fix full table scans on HTLC settlement hot path](https://github.com/lightningnetwork/lnd/pull/10619)
- [mod+multi: bump neutrino to v0.16.2 and btcwallet to 70a94ea](https://github.com/lightningnetwork/lnd/pull/10629)
