## <img src="https://github.com/input-output-hk/marlowe-ts-sdk/blob/0.4.0-beta/doc/image/logo-header.svg" height="24" /> What is Marlowe ?

Marlowe is a robust, open-source technology that provides a special purpose language describing asset flows on blockchain. As a special purpose, domain-specific language (DSL) it offers a higher-level model of contracts than other Cardnao languages, albeit in a more restricted domain. This means that we can provide safety guarantees, such as no assets being held in a script indefinitely, simply by the design of the language, and others, such as tools to fully analyze for contract faults before running a contract. 

Marlowe core technology has been audited, and it supports contracts on mainnet as well as in pre-production; its Runtime enables all the necessary on- and off-chain contract activity, including the tedious work of transaction construction; and the TypeScript SDK supports Marlowe as a component within a complete DApp. It is thus a smart contract technology that is complementary to Aiken, PlutusTx or Scalus, and abstracts away from the complexities of Cardano and provides a local, account-based model like Ethereum.

Marlowe is a fully open-source, community maintained project under the auspices of the Marlowe Language CIC (Community Interest Company), a uk-based non-profit organisation. The CIC is very grateful to IOG for supporting this transition process to independence. For more details see [this blog post](https://marlowe.iohk.io/blog/the-past-present-and-future-of-marlowe-a-journey-of-innovation-and-community-empowerment). Marlowe has received support from Catalyst Fund 13 to develop and implement [a novel Marlowe Oracle protocol](https://milestones.projectcatalyst.io/projects/1300131/milestones/3).

A longer overview of the status and plans for Marlowe can be found [here](https://github.com/marlowe-lang/.github/blob/main/Marlowe%20-Status-Report-Oct-2024.md).

## Marlowe repositories

Other developments run alongside this bid. We are working with IOG to move the Marlowe repositories to this independent GitHub organization, and to coordinate community activity and interest by means of a Marlowe Special Interest Group, supported by the Marlowe Language CIC. 

This Github organization will reference all the core projects related to Marlowe. The following IOG repositories will soon be transferred here : 

- [marlowe](https://github.com/input-output-hk/marlowe)
- [marlowe-cardano](https://github.com/input-output-hk/marlowe-cardano)
- [marlowe-plutus](https://github.com/input-output-hk/marlowe-plutus)
- [marlowe-playground](https://github.com/input-output-hk/marlowe-playground)
- [marlowe-runner](https://github.com/input-output-hk/marlowe-runner)
- [marlowe-ts-sdk](https://github.com/input-output-hk/marlowe-ts-sdk)
- [marlowe-scan](https://github.com/input-output-hk/marlowe-scan)
- [marlowe-starter-kit](https://github.com/input-output-hk/marlowe-starter-kit)
- [marlowe-doc](https://github.com/input-output-hk/marlowe-doc)
- [awesome-marlowe](https://github.com/input-output-hk/awesome-marlowe)
- [real-world-marlowe](https://github.com/input-output-hk/real-world-marlowe)
- [marlowe-order-book-swap](https://github.com/input-output-hk/marlowe-order-book-swap)
- [marlowe-ts-dapp-swap](https://github.com/input-output-hk/marlowe-ts-dapp-swap)
- [marlowe-payouts](https://github.com/input-output-hk/marlowe-payouts)
- [marlowe-token-plans](https://github.com/input-output-hk/marlowe-token-plans)
- [marlowe-agda](https://github.com/input-output-hk/marlowe-agda)
- [marlowe-actus-labs](https://github.com/input-output-hk/marlowe-actus-labs)
- [marlowe-lambda](https://github.com/input-output-hk/marlowe-lambda)
- [marlowe-hydra-poc](https://github.com/input-output-hk/marlowe-hydra-poc)
- [actus-core](https://github.com/input-output-hk/actus-core)
- [purescript-datetime-iso](https://github.com/input-output-hk/purescript-datetime-iso)
- [purescript-markdown](https://github.com/input-output-hk/purescript-markdown)
- [MIPs](https://github.com/input-output-hk/MIPs)
- [purescript-marlowe](https://github.com/input-output-hk/purescript-marlowe)
- [purescript-bridge-json-helpers](https://github.com/input-output-hk/purescript-bridge-json-helpers)
- [purescript-cardano-multiplatform-lib](https://github.com/input-output-hk/purescript-cardano-multiplatform-lib)
- [purescript-cardano-wallet-client](https://github.com/input-output-hk/purescript-cardano-wallet-client)
- [purescript-marlowe-runtime-client](https://github.com/input-output-hk/purescript-marlowe-runtime-client)
- [purescript-web-common](https://github.com/input-output-hk/purescript-web-common)
- [marlowe-cardano-minimal](https://github.com/input-output-hk/marlowe-cardano-minimal)

### New testing infrastructure

As Part of this transition, we are moving also our infrastructure, here are the new URLs : 

- [Marlowe Playground](https://playground.marlowe-lang.org)
<!--
- Runners
  - [preview.runner.marlowe-lang.org](https://preview.runner.marlowe-lang.org)
  - [preprod.runner.marlowe-lang.org](https://preprod.runner.marlowe-lang.org)
-->
- Runtime for preprod testnet:
  - [preprod.100.runtime.marlowe-lang.org/openapi.html](https://preprod.100.runtime.marlowe-lang.org/openapi.html)
  - [preprod.100.runtime.marlowe-lang.org/openapi.json](https://preprod.100.runtime.marlowe-lang.org/openapi.json)

<!--
  - [preview.100.runtime.marlowe-lang.org/openapi.json](https://preview.100.runtime.marlowe-lang.org/openapi.json)
-->

## <img src="https://raw.githubusercontent.com/CardanoSolutions/ogmios/master/.github/discord.svg" height="24" /> Community

Be part of the journey and join our welcoming community on [Discord](https://discord.gg/av37Cgc2).

## <img src="https://raw.githubusercontent.com/CardanoSolutions/ogmios/master/.github/twitter.svg" height="32" /> Follow us

Follow us on Twitter [@marlowe_io](https://twitter.com/marlowe_io) for updates and chats about the future of Marlowe.

