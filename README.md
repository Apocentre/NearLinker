!["Near Linker Logo](docs/images/NearLinker-Logo-Light.png#gh-dark-mode-only)
!["Near Linker Logo](docs/images/NearLinker-Logo-Dark.png#gh-light-mode-only)

<p align="center">
  <a aria-label="License" href="https://github.com/ExxaVerse/NearLinker/blob/main/LICENSE">
    <img alt="" src="https://img.shields.io/npm/l/next.svg?style=for-the-badge&labelColor=000000">
  </a>
  <a aria-label="Join the community on GitHub" href="https://github.com/ExxaVerse/NearLinker/discussions">
    <img alt="" src="https://img.shields.io/badge/Checkout%20the%20discussion-blue.svg?style=for-the-badge&labelColor=000000&logoWidth=20">
  </a>
</p>

# What is NearLinker?

NearLinker is an open source project that will allow developers to integrate [NEAR](https://near.org/) blockchain in games developed with Unreal Engine.

# Overview

The project is composed of two main components: the integration server and the Unreal Engine plugin. The integration server is created in [Node.js](https://nodejs.org/en/) and its main purpose is creating a communication channel with the NEAR blockchain. It will leverage [next-api-js](https://docs.near.org/docs/api/javascript-library) to establish communication with NEAR, while exposing REST API endpoints to be accessed from the outside. The Unreal Engine plugin will be configured by the developer to communicate directly with the NL server. It will be plugged inside Unreal Engine projects and will allow the features discussed below.

Smart contracts will be created and pushed separately on the NEAR blockchain. Implementation for smart contracts is done in Rust.

NearLinker will be featured in developing [Exxaverse](https://exxaverse.com/), a gladiator-themed play-to-earn game.

# Features

The following features will be implemented with the delivery of the project's MVP:

- Allowing users to view and transfer their fungible and non-fungible assets
- Real-time interaction with smart contracts
- Data encryption methods on both UE4 and integration server sides

More features will be disclosed closer to the full-launch.

# Architecture

![NearLinker Architecture](docs/images/NearLinker-Architecture-Dark.png#gh-light-mode-only)
![NearLinker Architecture](docs/images/NearLinker-Architecture-Light.png#gh-dark-mode-only)

Architecture breakdown:

- `NEAR blockchain` - the main data storage
- `NodeJS Integration Server` - communicates with the NEAR blockchain through specific libraries
- `RUST Smart Contracts` - smart contracts are written in Rust and deployed directly on the blockchain
- `UE Clients` - games developed in Unreal Engine that use the NearLinker plugin to connect to the blockchain

# FAQ & Contact
