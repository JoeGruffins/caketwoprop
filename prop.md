## Introduction

Decred is finally on cake wallet. This is a followup now that the first proposal is finished. This proposal aims to make decred on cake more user friendly.

## Main objectives

There are three main objectives we want to accomplish with this proposal.

1. Speed up initial sync. We have a rough plan to cut off 300mb from the initial sync by ignoring cFilters before the wallet birthday. This should half initial sync times, but will take a lot of changes in dcrwallet and is not a small task.

2. Refactor and version libwallet. This library was originally created by @itswisdomagain for dcr, ltc, and btc. However we decided to throw out ltc and btc and focus on dcr. It still needs some refactoring to remove some of the abstraction layers that were needed for three wallet types. It also lacks versioning which we want to figure out.

3. Restore from hardware support. We are already on ledger so this should not be a problem.

## Bug support

As people actually use the wallet we expect bugs to appear. This gives us funding to fix those. One currently known bug that needs investigation is that decred is not working on the Graphene OS which will be looked into.

## Discretionary

Will be used on testing devices.

## Who

To be done by any interested decred contractors, especially Wisdom, Dreacot, Philemon, and Joe.

## Work

We anticipate costs in the range of **60k USD** and expect to have the main objectives done in 8 months.

| Item                                        | How Much       | FTE Weeks |
|---------------------------------------------|---------------:|----------:|
|  Main objectives                            | 30k            | 12        |
|  Bug support                                | 20k            | 8         |
|  Discretionary                              | 10k            | 4         |
| **Total**                                   | **60k**        | 24        |
