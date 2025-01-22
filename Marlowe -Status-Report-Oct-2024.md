# Marlowe Platform status report

## October 2024, updated January 2025

# What is Marlowe?

Marlowe is a high-level smart contract language, designed to describe asset flows on blockchain. Marlowe embodies a local, account-based model, and runs equally well on UTxO and account-based chains like Ethereum. Marlowe describes fully distributed interactions between contract participants, mediated by the underlying blockchain. 

Contracts written in Marlowe automatically provide safety guarantees, such as no assets being held in a script indefinitely, and no script running forever. Marlowe contracts can also be fully analysed for contract faults before running them. The Marlowe on-chain validators have been audited, and Marlowe supports contracts on the Cardano mainnet as well as in pre-production.Ma

# What is the Marlowe Platform?

The Marlowe Platform provides all that is needed to build and run complete DApps on Cardano, leveraging the guarantees provided by Marlowe smart contracts, and integrating with Web3 workflows through a TypeScript SDK. The platform Includes:

* The Marlowe Runtime, which supports all the necessary on- and off-chain contract actions, including the tedious work of transaction construction and tracking contract activity by other participants.  
* The Marlowe TypeScript SDK fully integrates Marlowe as a component within a complete DApp, including contract creation and initialization, as well as execution.  
* The Marlowe Playground provides the environment for learning Marlowe, through its Blockly representation, as well as simulation and analysis of contracts as they are developed.  
* End-to-End DApp examples, developed in collaboration with Gimbalabs with Catalyst Fund 12 support, and designed to make access to the Marlowe Platform as straightforward as possible.  
* Other components supporting free-standing execution of Marlowe smart contracts, including the Marlowe Runner and the Marlowe CLI.

The Marlowe Platform is 100% Open Source, (C) Marlowe Language CIC, a non-profit organisation to foster and sustain Marlowe and its ecosystem.

# Who can use Marlowe?

DApp developers, SMEs and enterprises will use the Marlowe Platform to develop Cardano-based DApps. The platform makes development as accessible as possible to the developer community, as well as providing key components, such as oracles, used in many DApps. 

Individual end users are also able to execute Marlowe contracts directly on the Cardano blockchain, using facilities provided by the Marlowe Runner and CLI. This directly supports DeFi interactions including peer-to-peer loans and escrow facilities.

# Why should I use Marlowe?

The Marlowe Platform offers an easier and more effective route to DApp development than Aiken or PlutusTx, as long as the core functionality of the DApp can be described by means of Marlowe contracts. 

Each Marlowe contract has a predetermined, finite, set of roles, and behaviour that is guaranteed to terminate, but it is crucial to realise that a DApp using the platform can create and execute multiple Marlowe contracts on the fly for particular use cases. For example, an escrow service DApp can generate a new Marlowe contract for each particular use of the service, and that contract will provide a guarantee of termination and no asset retention for each such use.

Marlowe provides the infrastructure for developers to build DApps using familiar technology,  TypeScript and related platforms, to build complete DApps. Where it can be used it provides

* Lower barrier to entry of writing Cardano DApps: the platform integrates Marlowe as a first-class component in Web3 development.  
* Greater productivity because the language is higher level: Marlowe contracts describe the flows of assets, rather than requiring details of blockchain transactions and so forth.  
* The Runtime supports building and executing Marlowe contracts as an integral component of a running DApp.  
* Each Marlowe contract instance gives a high level of safety guarantees, by design. 

# Is Marlowe ready to use?

Marlowe is ready to use. Marlowe runs on mainnet, it is supported by online services (e.g [Marlowe Playground](https://playground.marlowe-lang.org/), [Marlowe Runner](https://preview.runner.marlowe-lang.org/)). 

It can also be seen in action in the example provided by the [Marlowe PBL 2025](https://projectcatalyst.io/funds/12/f12-cardano-open-developers/marlowe-pbl-2025) project and some prototypes developed by the Core Marlowe Team (e.g [Token Plans](https://github.com/input-output-hk/marlowe-vesting), [Payouts](https://github.com/input-output-hk/marlowe-payouts) and the [Order Book Swap](https://github.com/input-output-hk/marlowe-order-book-swap) Prototype). 

However, it still needs to evolve from an MVP to a fully refined product, with the most highly requested improvements being improvements to the Marlowe validator to support Contract Execution Optimization, and, in the longer term to support Seamless DApp Integration of Deep Contracts, including Merkelization support.

The Roadmap below outlines the ways that we aim to improve Marlowe, and the timeline for the delivery. The Marlowe Platform proposal(s) submitted to Catalyst Fund 13 seeks funding to implement the key aspects of the roadmap in 2025\.

# Marlowe Roadmap

### Collaboration: end-to-end example

The Marlowe team is working with the Gimbalabs Catalyst Fund 12 (CF12) funded project [Marlowe PBL 2025](https://projectcatalyst.io/funds/12/f12-cardano-open-developers/marlowe-pbl-2025) to ensure that there is a prototype, end-to-end example of development of a DApp using the Marlowe Platform as it stands. Through 2025 this will be upgraded in line with ongoing developments of the Platform and the language. 

### Marlowe 2025: Oracle Protocol, Design and Implementation

The current oracle systems on Cardano operate predominantly on a fixed, push-based model, which limits the ability to meet diverse and less commonly used data needs for smart contracts. Our solution, the Marlowe Oracle Protocol, aims to solve this by shifting towards a pull-based model, where oracles respond dynamically to on-chain data requests, ensuring better adaptability and data coverage for a wider array of contracts.

Our approach is centered around enhancing flexibility, transparency, and simplicity. We want to make the process of using oracles in smart contracts much more accessible to developers, whether they are experienced with Cardano tools or are just getting started with Marlowe, Aiken, or PlutusTx. The protocol will also include user-friendly tools, developed in TypeScript, Rust, and Haskell, to facilitate oracle accessibility for the end users and simplify integrations for developers as well as data providers. This initiative is funded under Catalyst Fund 13 as project 1300131, starting by the end of January 2025. The high-level objectives of the project are

* Formalize Marlowe Oracle Specification
* Marlowe Validator and Runtime Adaptations to support the oracle protocol
* Deliver a complete DApp supporting the full Marlowe Oracle Service
* Provide and document an integration of the Oracle protocol into the Marlowe TypeScript SDK
* Provide Aiken Integration for the Oracle service
* Documentation and Marlowe DApp Starter Kit Integration

The full milestones of the project are listed [here](https://milestones.projectcatalyst.io/projects/1300131/milestones),




### Marlowe 2025: enhanced Marlowe Platform

This roadmap aims to unlock the latent potential of the Marlowe platform by implementing critical updates to the Marlowe validator and tech stack, making these advanced capabilities accessible and of benefit to a wider audience. 

* Marlowe DApp Starter Kit

  Building on the end-to-end example, the team will deliver the Marlowe DApp Starter Kit (DSK), that will consolidate the documentation, examples and tutorials into an end-to-end guide to design and implementation, through to deployment and maintenance, of DApps that leverage Marlowe tools and capabilities. The DSK will include comprehensive support materials such as tutorials, readily available software packages, and pre-built binaries to ensure ease of implementation. The initial DSK will be delivered early in the project, and incrementally enhanced with new technologies as these are developed. 

* Validator Enhancements

  It is proposed to  implement targeted changes to the current validator, designed to significantly reduce the on-chain execution costs for specific contracts and Marlowe idioms.  This process will not only improve efficiency but also expand capabilities, including the integration of off-chain micropayment channels into our framework. Specific changes will include bypassing the double satisfaction check for whitelisted scripts to eliminate extra INotify transactions and enhancing Marlowe validators to enable automatic withdrawals through direct role payouts to wallet addresses. These changes will be integrated into the entire Marlowe toolchain, and will be illustrated in a suite of DApp prototypes, each thoroughly documented and made accessible through the marlowe-ts-sdk.

* Configurable Runtime Fee Mechanism

  To incentivize infrastructure providers and SPOs to adopt and integrate Marlowe into their services, it is proposed to introduce a configurable fee mechanism within the Marlowe Runtime. This backend enhancement will support the safe execution of Marlowe contracts via web applications, bolstered by a new Tx validation layer in the TypeScript client library. This layer will ensure secure interactions, even with untrusted backends, facilitating a wider distribution and adoption of Marlowe technology.

* Seamless DApp Integration of Deep Contracts (Merkleized Contracts)   
    
  Integrating Marlowe contract execution into a DApp should involve managing a state machine with ease, where contract designers define steps and transitions. This allows contract integrators to focus on business logic and create a custom UI. However, Marlowe currently lacks higher-level abstractions to achieve this smoothly. Merkleization examples are experimental and not well integrated into runtime APIs, and there is no annotation system to easily track contract execution and available transitions.

The Marlowe team has submitted two Catalyst Fund 13 bids to support work on [platform enhancements](https://cardano.ideascale.com/c/idea/132547) and [the Marlowe oracle protocol](https://cardano.ideascale.com/c/idea/131188).

### 2025: Marlowe Language V2

Concurrently with enhancing the Platform, it is planned to review the current design of the Marlowe Language, and to design and implement a second major version of the language, Marlowe V2. Working with the community we will collect and prioritise proposals for Marlowe V2, prototype them in the reference Agda implementation, and based on the results, design the revised language.

The enhancements delivered here will aim to improve the language in these ways:

* **Simplification** of aspects of the original language. This might include simplifying the “When” construct so that the contract will by default close on timeout. Generalising some constructs, such as a “When” that awaits a set of actions, could substantially simplify the expression of a common programming pattern.  
* Making the language **more expressive**. This could include adding new control constructs, such as bounded loops, and primitives, e.g. for crypto operations. It would also include conceptual additions, such as sub-languages for time arithmetic or token minting.  
* Improving the **scalability** of the language: an example of this would be to change the behaviour of a contract on close to optimise performance with larger numbers of contract participants.  
* Addressing the **security** of the language, which could be improved by checking types of values, so that e.g. addition only takes place between the same “kind” of number.

This is the subject of this [Catalyst proposal](https://cardano.ideascale.com/c/idea/131139).

# How is Marlowe administered and managed?

Marlowe is owned and managed by the non-profit organisation Marlowe Language CIC, with UK company number 16010921\. This Community Interest Company exists to 

* Promote and assist in the administration and establishment of the community of users and developers of the Marlowe language and the Marlowe Platform, both of which are available as Open Source software.  
* Support the development, maintenance, education and training in the Marlowe language and platform.   
* Host the Marlowe open source software on its repositories, and maintain an online presence for the Marlowe ecosystem including web pages, documentation, blogs, tutorials and videos.  
* Organise face to face meetings and tutorials, in order to foster community cohesion and growth.


The CIC provides benefit to the wider Marlowe community by:

* Ensuring that the software is maintained in an up-to-date state, consistent with other open source technologies on which it depends.  
* Ensuring that the community itself is sustained, and that new members and developers are onboarded and trained, so that maintenance and enhancement of the software by open source contribution will be maintained.  
* Through making available educational and other materials, ensuring that the community can keep itself up to date with technology developments, as well as educating other end users in how Marlowe can be employed in practice. This will ensure that Marlowe’s benefits are taken up by as broad a group as possible.  
* Ensuring that the views of the community are sought and shape roadmaps and plans for the future development of Marlowe, so that it is most likely to develop in ways that most benefit the greatest number of community members.

# How can I support Marlowe?

You can help Marlowe by joining the community at [Marlowe Special Interest Group](https://discord.com/channels/826816523368005654/1239607206446497843), and beginning to contribute to the ecosystem. You can do that by becoming a contributor to the core language and its infrastructure, including the various components of the Marlowe Platform, by developing example and use cases, by authoring educational materials, and by integrating Marlowe with other technologies and blockchains. 

Crucially, you can support the ***Marlowe 2025*** bids for Catalyst Fund 13:

* [Marlowe Version 2](https://cardano.ideascale.com/c/idea/131139)  
* [Developer-Driven Platform Enhancements](https://cardano.ideascale.com/c/idea/132547)   
* [Oracle Protocol, Design and Implementation](https://cardano.ideascale.com/c/idea/131188) 

