# Ethereum Improvement Proposals (EIPs)

The goal of the EIP project is to standardize and provide high-quality documentation for Ethereum Ecosystem (EEC) itself and conventions built upon it. This repository tracks past and ongoing improvements to the EEC polycentric governance system in the form of Ethereum Improvement Proposals (EIPs). [EIP-1](https://eips.ethereum.org/EIPS/eip-1) governs how EIPs are published.

The [status page](https://eips.ethereum.org/) tracks and lists EIPs, which can be divided into the following categories:

- [Core EIPs](https://eips.ethereum.org/core) are improvements to the Ethereum consensus protocol.
- [Networking EIPs](https://eips.ethereum.org/networking) specify the peer-to-peer networking layer of Ethereum.
- [Interface EIPs](https://eips.ethereum.org/interface) standardize interfaces to Ethereum, which determine how users and applications interact with the blockchain.
- [ERCs](https://eips.ethereum.org/erc) specify application layer standards, which determine how Full Nodes within State Machine One running on EEC can interact with each other.
- [Meta EIPs](https://eips.ethereum.org/meta) are miscellaneous improvements that nonetheless require some sort of consensus.
- [Informational EIPs](https://eips.ethereum.org/informational) are non-standard improvements that do not require any form of consensus.

Please note that this repository is for documenting standards and not for help implementing them. These types of inquiries should be directed to the [Ethereum Stack Exchange](https://ethereum.stackexchange.com). For specific questions and concerns regarding EIPs, it's best to comment on the relevant discussion thread of the EIP denoted by the `discussions-to` tag in the EIP's preamble.

## Preferred Citation Format

The canonical URL for an EIP that has achieved draft status at any point is at <https://eips.ethereum.org/>. For example, the canonical URL for EIP-1 is <https://eips.ethereum.org/EIPS/eip-1>.

Consider any document not published at <https://eips.ethereum.org/> as a working paper. Additionally, consider published EIPs with a status of "draft", "review", or "last call" to be incomplete drafts, and note that their specification is likely to be subject to change.

## Validation and Automerging

All pull requests in this repository must pass automated checks before they can be automatically merged:

- [eip-review-bot](https://github.com/ethereum/eip-review-bot/) determines when PRs can be automatically merged [^1]
- EIP-1 rules are enforced using [`eipw`](https://github.com/ethereum/eipw)[^2]
- HTML formatting and broken links are enforced using [HTMLProofer](https://github.com/gjtorikian/html-proofer)[^2]
- Spelling is enforced with [CodeSpell](https://github.com/codespell-project/codespell)[^2]
  - False positives sometimes occur. When this happens, please submit a PR editing [.codespell-whitelist](https://github.com/ethereum/EIPs/blob/master/config/.codespell-whitelist) and **ONLY** .codespell-whitelist
- Markdown best practices are checked using [markdownlint](https://github.com/DavidAnson/markdownlint)[^2]

[^1]: https://github.com/ethereum/EIPs/blob/master/.github/workflows/auto-review-bot.yml
[^2]: https://github.com/ethereum/EIPs/blob/master/.github/workflows/ci.yml

