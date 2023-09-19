# IPFS Gateway API

Leto's IPFS Gateway is a comprehensive, lightweight, and fast API that respects your privacy. It enables you to access InterPlanetary File System (IPFS) content anonymously and offers a metric-based approach to analyze usage patterns. The image below illustrates the structure of the Proxy Gateway Architecture:

![Proxy Gateway Architecture](https://user-images.githubusercontent.com/30084404/225565389-d78d75a7-7ee7-44c8-8ece-3793928c0f30.png)

## Core Features

Here are the principal features offered by our IPFS Gateway:

* **Anonymity**: Our Gateway ensures you can access IPFS content without revealing your identity.
* **Privacy**: No logging of IP addresses or personal information.
* **Performance**: The Gateway is lightweight, fast, and easy to initialize.
* **Metrics**: We perform analyses based on the frequency and timing of CID requests.

## Switching Gateways

To switch from your current IPFS Gateway to ours, all you need to do is change your Gateway address to the Leto Gateway, available at `leto.gg/ipfs/"cid"`.

## Accessing IPFS via HTTP

Accessing IPFS data via HTTP is straightforward, particularly when utilizing an IPFS HTTP gateway. As a decentralized peer-to-peer network, IPFS simplifies data retrieval. We'll be using the Leto.gg's gateway in this guide, built on the Web3.Storage Superfast Gateway, offering anonymous metrics alongside data provision.

Upon storing data using the [web3.storage client](https://web3.storage/docs/how-tos/store/), the `put` method returns an [IPFS content identifier (CID)](https://docs.ipfs.io/concepts/content-addressing/) string. This CID corresponds to an IPFS directory containing files sent via the `put` method.

Here's how to leverage these CIDs:

* Point your application or program to the data in the Web3.Storage infrastructure using the respective CID.

> **Note:** The w3link (https://ipfs.w3s.link/\*) imposes a rate limit of 200 requests per minute per IP.
