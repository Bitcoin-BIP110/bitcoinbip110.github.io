# Bitcoin BIP110

[bitcoinbip110.org](https://bitcoinbip110.org/) is a technical reference and network observatory for Bitcoin BIP110, the independent chain intended to continue the historical BIP 110 enforcement branch through a BLAKE2b proof-of-work implementation being developed from Bitcoin Knots.

The site documents the chain split, software development, network status, protocol parameters, compatibility evidence, and operational guidance for node operators, miners, wallet developers, researchers, exchanges, and custodians.

## Network overview

- **Origin chain:** Bitcoin
- **Last shared block height:** `961,631`
- **First divergent height:** `961,632`
- **Historical enforcement-branch proof of work:** SHA-256d
- **Planned proof of work:** BLAKE2b header v2
- **Proposed display name:** Bitcoin BIP110
- **Proposed ticker:** BIP110
- **Asset type:** Native coin, not a token

Bitcoin mainnet and the BIP 110 enforcement branch share the Bitcoin ledger through block 961,631. At height 961,632, BIP 110 enforcing nodes rejected a non-signaling Bitcoin mainnet block and accepted a competing bit-4-signaling block. The resulting enforcement branch later became the basis for the proposed Bitcoin BIP110 BLAKE2b continuation.

The BLAKE2b transition is separate from the original [BIP 110](https://bips.dev/110/) specification. Final mainnet activation parameters must be confirmed from signed release source before they are treated as operational.

## Site sections

- **Overview:** Current project status and the distinction between BIP 110, its enforcement branch, Bitcoin mainnet, and Bitcoin BIP110
- **History:** The original proposal, the split at height 961,632, and the early SHA-256d branch
- **Timeline:** Dated events with verification status and primary sources
- **Technical:** Consensus, proof-of-work, mining, replay behavior, and integration information
- **Sources:** Primary references used throughout the site

## Editorial standard

Technical and historical claims should link to primary sources wherever possible. Updates should:

- Distinguish proposals, open pull requests, tagged releases, scheduled activations, and observed network events
- Attach dates to changing development and network-status claims
- Use exact block heights, hashes, release tags, and commit references
- Mark unknown parameters as pending instead of inferring values
- Treat hardware compatibility as unconfirmed until demonstrated for a specific miner, firmware, header profile, and mining stack
- Keep BIP 110, the historical enforcement branch, Bitcoin mainnet, and Bitcoin BIP110 terminologically distinct

Material changes to chain status or mainnet parameters should be supported by independently verifiable node data or signed, versioned source.

## Primary references

- [BIP 110: Reduced Data Temporary Softfork](https://bips.dev/110/)
- [Bitcoin Knots](https://bitcoinknots.org/)
- [Bitcoin Knots PR #359: BLAKE2b proof of work](https://github.com/bitcoinknots/bitcoin/pull/359)
- [Bitcoin Knots PR #357: opt-in unified signature hash](https://github.com/bitcoinknots/bitcoin/pull/357)
- [Last shared block at height 961,631](https://mempool.space/block/00000000000000000000807f9dc917442a67910426d79ebb2f8aa2149327ce8a)
- [First BIP 110 enforcement-branch block at height 961,632](https://mempool.guide/block/0000000000000000000169eb6f811ddbd0daf343af7b62180cdb13e7c78dbc16)

## Contributing

Corrections and sourced updates are welcome through GitHub issues or pull requests. Include the primary source, the date observed, and the exact statement or page that should change.
