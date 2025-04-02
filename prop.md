## Introduction

Decred is finally on cake wallet. This is a followup now that the [first proposal](https://proposals.decred.org/record/b3bdacb) is finished. This proposal aims to make decred on cake more user friendly.

## Main objectives

There are four main objectives we want to accomplish with this proposal.

1. Speed up initial sync. We have a rough plan to cut off 300mb from the initial sync by ignoring cFilters before the wallet birthday. This should half initial sync times, but will take a lot of changes in dcrwallet and is not a small task.

2. Refactor and version libwallet. This library was originally created by @itswisdomagain for dcr, ltc, and btc. However we decided to throw out ltc and btc and focus on dcr. It still needs some refactoring to remove some of the abstraction layers that were needed for three wallet types. It also lacks versioning which we want to figure out.

3. Add restore from hardware support. We are already on ledger so this should not be a problem.

4. Add decred to btc pay server so that it can be used in Cake Pay. More below...

## Integrate DCR to BTCPay Server for use with Cake Pay

[BTCPay Server](https://btcpayserver.org/) is an open-source, self-hosted payment processor for cryptocurrencies. It allows merchants and users to accept payments directly, without intermediaries, offering full control, no transaction fees (beyond network costs), and enhanced privacy. It’s customizable, supports multiple cryptocurrencies, and integrates with wallets and e-commerce platforms, making it a powerful tool for decentralized finance.

[Cake Pay](https://cakepay.com/) is a service by Cake Wallet that lets you buy gift cards with supported cryptocurrencies. It allows users to spend crypto at hundreds of merchants worldwide by purchasing gift cards instantly, often with small discounts (1-3%). Accessible via the Cake Wallet app or web, it’s designed for easy, practical crypto use. BTCPay Server is how Cake Pay processes payments.

With Decred now available on Cake Wallet, the next logical step is to ensure it can be used with Cake Pay by completing a BTCPay Server integration.

<em>We will do the work but as for **when** BTCPay will merge our prs is not up to us.</em>

## Bug support

As people actually use the wallet we expect bugs to appear. This gives us funding to fix those. One currently known bug that needs investigation is that decred is not working on the Graphene OS with some settings enabled, which will be looked into.

## Discretionary

Will be used on testing devices.

## Who

To be done by any interested decred contractors, especially Wisdom, Dreacot, Philemon, and Joe.

## Work

We anticipate costs in the range of **80k USD** and expect to have the main objectives done within in 12 months.

| Item                                        | How Much       | FTE Weeks |
|---------------------------------------------|---------------:|----------:|
|  Main objectives                            | 50k            | 20        |
|  Bug support                                | 20k            | 8         |
|  Discretionary                              | 10k            | 4         |
| **Total**                                   | **80k**        | 32        |
