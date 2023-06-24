---
title: "Hashing Algorithms: SHA and MD Explained in Layman's Terms"
datePublished: Sat Jun 24 2023 05:06:48 GMT+0000 (Coordinated Universal Time)
cuid: clj9jgxba00060al9hn7ke7aj
slug: hashing-algorithms-sha-and-md-explained-in-laymans-terms
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1687583187109/72e000b8-a294-42a4-aa23-d5a554af7c94.png
tags: 2articles1week

---

# Introduction:

In today's digital world, where data security is of utmost importance, understanding hashing algorithms is essential. In this blog post, we will explore two commonly used hashing algorithms: Secure Hash Algorithm (SHA) and Message Digest (MD). We will delve into the inner workings of each algorithm in simple terms, enabling a better understanding of their functionalities and use cases.

## Understanding Secure Hash Algorithm (SHA):

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1687581609392/a26a48a7-19a2-48b3-a18f-4dd42de4e1fd.png align="center")

The Secure Hash Algorithm, commonly known as SHA, is a family of cryptographic hash functions. In simple words, a hash function is like a "magic box" that takes an input (data) and produces a fixed-length output (hash value), which is unique to that input.

1. **SHA-1:** SHA-1 is an earlier version of SHA but is no longer considered secure due to vulnerabilities. It generates a 160-bit hash value, which is a unique representation of the input data. However, collision attacks can occur, meaning two different inputs may produce the same hash value.
    
2. **SHA-2:** SHA-2 is a set of hash functions that offer improved security over SHA-1. It includes different variants such as SHA-224, SHA-256, SHA-384, and SHA-512. The numbers in the names represent the lengths of the hash values they produce. For example, SHA-256 generates a 256-bit hash value. The larger the hash value, the more secure it is against attacks.
    
3. **SHA-3:** SHA-3 is the latest addition to the SHA family. It offers a different design approach compared to SHA-2. Like SHA-2, it produces hash values of various lengths, providing robust security and improving resistance against potential attacks.
    

### Applications of SHA:

1. **Digital Signatures**: SHA algorithms are widely used in digital signature schemes to ensure data integrity and authentication. By generating a unique hash value for a document or message, SHA algorithms allow recipients to verify that the content has not been modified during transmission.
    
2. **Password Storage:** SHA algorithms, especially the SHA-2 family, are commonly employed for securely storing passwords. Instead of storing the actual passwords, their hash values are stored. During authentication, the input password is hashed and compared with the stored hash value to validate the user's credentials.
    
3. **Blockchain Technology:** SHA algorithms, particularly SHA-256, are integral to blockchain technology. They provide the cryptographic backbone for mining new blocks and verifying the integrity of existing blocks in a decentralized and secure manner.
    

## Exploring Message Digest (MD) Algorithms:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1687582663956/41543192-d643-41b0-aad8-ddf37ab67bf7.png align="center")

Message Digest (MD) algorithms are another set of hash functions, but they are generally considered less secure than SHA algorithms. Let's look at two commonly known MD algorithms:

1. **MD5**: MD5 is a widely used algorithm that generates a 128-bit hash value. However, it is no longer recommended for cryptographic purposes due to its vulnerabilities. MD5 is prone to collision attacks, where two different inputs can produce the same hash value, making it unreliable for data integrity verification.
    
2. **MD4:** MD4 is an earlier version of MD algorithms, also producing a 128-bit hash value. Similar to MD5, MD4 is considered insecure due to its vulnerabilities to collision attacks.
    

### Applications of MD5:

1. **Checksums:** MD5 is commonly used to generate checksums for verifying the integrity of files. By calculating the MD5 hash value of a file before and after transmission, one can compare the checksums to determine if the file has been altered or corrupted.
    
2. **Data Deduplication:** In certain scenarios, MD5 is used for data deduplication, which involves identifying and eliminating duplicate copies of data. By calculating the MD5 hash values of data chunks or files, duplicates can be identified and eliminated, optimizing storage space.
    

It's important to note that the use of MD5 for cryptographic purposes, such as password storage or digital signatures, is strongly discouraged due to its vulnerabilities to collision attacks.

### Basic Overview of How These Algorithms Work

Both SHA and MD algorithms follow similar steps to produce hash values:

1. **Breaking Down the Data:** The input data is divided into smaller blocks to process efficiently.
    
2. **Data Transformation:** Each block undergoes a series of complex mathematical operations, including bitwise operations, logical functions, and modular arithmetic. These operations create a unique representation of the input data.
    
3. **Output Compression:** The intermediate hash values generated for each block are combined and compressed to produce a final hash value. This value is the unique fingerprint of the input data.
    

## Conclusion

Understanding hashing algorithms such as SHA and MD is crucial for anyone involved in data security. SHA algorithms, particularly SHA-2 and SHA-3, offer improved security compared to the older SHA-1. While MD algorithms served their purpose in the past, they are now considered less secure due to their vulnerabilities.

By grasping the basics of these algorithms, we can better protect sensitive data, ensure data integrity, and contribute to a more secure digital landscape.

Remember, in the ever-evolving world of cybersecurity, staying informed and adopting robust security measures is key.

Happy hashing and secure computing!

references:

[https://www.researchgate.net/figure/Block-Diagram-of-MD5-Algorithm-17\_fig1\_329353052](https://www.researchgate.net/figure/Block-Diagram-of-MD5-Algorithm-17_fig1_329353052)

[https://www.semanticscholar.org/paper/High-Throughput-Implementation-of-MD5-Algorithm-on-Hu-Ma/f5e59f3696df493904dc8dd4e4e2b18adf93dfd6/figure/1](https://www.semanticscholar.org/paper/High-Throughput-Implementation-of-MD5-Algorithm-on-Hu-Ma/f5e59f3696df493904dc8dd4e4e2b18adf93dfd6/figure/1)

[https://ecomputernotes.com/computernetworkingnotes/security/sha-1](https://ecomputernotes.com/computernetworkingnotes/security/sha-1)