---
title: "What the Heck is Proof of History"
seoTitle: "Proof of History Consensus Protocol: Solving Blockchain's Bottleneck"
seoDescription: "Proof of History (PoH) is a consensus protocol that uses a time delay function to establish the order of transactions on a blockchain. PoH enables fast and"
datePublished: Thu May 04 2023 17:11:04 GMT+0000 (Coordinated Universal Time)
cuid: clh9dvw5h000009mjcehidsok
slug: what-the-heck-is-proof-of-history
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1682803661921/f056efe1-028f-4b18-9af8-d90685c492fa.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1683220070392/96d17db7-52d4-4124-9ca3-8b215ad9a797.png
tags: blockchain, web3, blockchain-technology, solana, proofofstake

---

In 2017 **Anatoly Yakovenko** published a whitepaper describing a technique for keeping time between different nodes that do not trust each other. It is called **Proof of History**. Blockchain systems like Bitcoin and Ethereum don't have a clock and they struggle to scale beyond 20tps (transaction per second) when centralized payment systems like Visa have a transaction speed of 2400tps and can peak up to 64000tps without a clock. **The main problem was getting computers that don't trust each other to agree on a time**, when Anatoly solved the problem the resulting cluster became 10,000 times faster. Conceptually, PoH is a way to cryptographically prove the passage of time, this way the entire network can forget about verifying the temporal claims of nodes and also provides fault tolerance in the network by providing an eventual consistency, It is done by the verifiable delay function. PoH is an improvement on the Proof of Work algorithm, Validator nodes still need to ensure transactions are legitimate but with timestamp and ordering, transactions can be validated faster which removes the PoW bottleneck. Using the PoH concept Solana was launched in June 2021. It is a Layer 1 chain, which means it provides the foundation of a block network, on top of which another Layer 2 networks can be built.

The time delay function is a core component of the Proof of History (PoH) consensus protocol, used to establish the order of transactions on a blockchain. The function takes a unique input value, such as the hash of the previous block, and applies a computationally intensive mathematical operation to it. The output is a random number that serves as a unique and verifiable measure of time.

Here is some pseudocode to illustrate how the time delay function works:

```bash
function timeDelay(inputValue):
  hashValue = hash(inputValue)
  nonce = 0
  while true:
    result = hash(hashValue + nonce)
    if result meets certain criteria:
      return result
    nonce++
```

In this pseudocode, the `hash` function takes an input and returns a hash value. The `nonce` variable is a number that is incremented each time the `hash` function is called. The `while` loop continues indefinitely until a valid result is found.

The criteria for a valid result depend on the specific implementation of the PoH consensus protocol. Generally, the result should be a number that falls within a certain range or has a certain number of leading zeros when represented in binary format.

The computational intensity of the time delay function is achieved by requiring the `while` loop to run for a significant amount of time before a valid result is found. This delay ensures that all nodes in the network have a consistent view of the blockchain's history.

In summary, the time delay function is a key component of the PoH consensus protocol that uses a computationally intensive mathematical operation to produce a verifiable and unique measure of time. The function's resistance to manipulation is achieved by requiring a significant amount of time to compute and by using specific criteria to determine a valid result.

## Some features of Solana apart from fast transaction speed are:

**1\. Censorship resistance:** Solana has rotating validator nodes, and for each validator, smart algorithms find the minimum number of nodes that need to be compromised to censor the network.

**2\. High scalability:** Solana has a high network traffic volume and is the best fit for enterprise-level applications while delivering a satisfying user experience.

**3\. interoperability:** Solana has layered architecture which makes it interoperable with other blockchains. Proof of History has one huge drawback which is a lot of power if the hardware and data capacity from validators is required to run it successfully.

Proof of History (PoH) is a revolutionary concept in the blockchain world that has the potential to solve one of the major bottlenecks that current blockchain systems face. By cryptographically proving the passage of time, PoH enables fast and secure transaction processing without relying on a centralized clock or a Proof of Work algorithm. The success of PoH can be seen in the launch of Solana, which is quickly gaining popularity as a high-performance blockchain.

One of the major advantages of PoH is its ability to provide fault tolerance in the network. By ensuring eventual consistency, PoH eliminates the need for nodes to verify the temporal claims of other nodes, which greatly reduces the computational burden on the network. Additionally, PoH allows for faster transaction validation by providing timestamps and ordering information.

Solana, the Layer 1 chain built using the PoH concept, has many advantages over other blockchain systems. Its censorship resistance is ensured by the rotating validator nodes, which require a minimum number of compromised nodes to censor the network. Solana also boasts high scalability, making it ideal for enterprise-level applications, and its layered architecture allows for interoperability with other blockchains.

**Downsides:** However, it is important to note that PoH does have a drawback. Running PoH successfully requires a significant amount of hardware and data capacity from validators, which can result in high power consumption. Despite this drawback, PoH remains a promising solution for achieving fast and secure transaction processing in decentralized networks.