# Leto's IPFS Gateway API

Here's the breakdown for Leto's IPFS Gateway. Our gateway keeps tabs on the volume of requests for IPFS objects or Content Identifiers (CIDs), but don't worry - it's all anonymous. We created the CID metrics feature to only track frequently requested CIDs, giving us a peek into usage patterns.

![Proxy Gateway Architecture](https://user-images.githubusercontent.com/30084404/225565389-d78d75a7-7ee7-44c8-8ece-3793928c0f30.png)

## Main Features

- Use the Gateway to get IPFS content without revealing your identity.
- We respect your privacy - no IP addresses or personal info logged.
- It's light, fast, and a breeze to get running.

**Tracking:** The gateway remembers every CID request, timestamp included.
**Metrics:** We crunch numbers based on CID request frequency and timing.
**Data Export:** Need to analyze metrics further? Export them as CSV, JSON, and more.

## Switching Gateways

Already using an IPFS Gateway? Switching to ours is as simple as changing your Gateway address to the Leto Gateway, found at "leto.gg/ipfs/cid".

## Accessing IPFS via HTTP

IPFS data is easy to get especially when using a IPFS HTTP gateway, since IPFS is a decentralized peer-to-peer network. In this guide, we'll use Leto.gg's gateway, which is built on the Web3.Storage Superfast Gateway. Alongside giving you your data, it offers anonymous metrics.

When you [store data with the web3.storage client](https://web3.storage/docs/how-tos/store/), the put method spits back an [IPFS content identifier (CID)](https://docs.ipfs.io/concepts/content-addressing/) string. This CID leads to an IPFS directory full of files you sent via the put method.

- Use these CIDs to point your program or app to the data in the Web3.Storage infrastructure.

Just a heads up, w3link (https://ipfs.w3s.link/*) has a rate limit of 200 requests per minute per IP.
