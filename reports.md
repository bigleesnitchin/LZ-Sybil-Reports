This report contains 22 clusters, exceeding the character limit for issue submissions on GitHub. Therefore, the later clusters and their descriptions will be moved to an external repository, which will remain unedited after the report is submitted.

Each cluster in this report is independent, with its own description and argumentation. Ideally, each cluster would have its own issue, but this would likely result in my account being flagged for spam by GitHub.

Thank you for understanding and accommodating these adjustments due to the report's length.















# Comprehensive Approach and Walkthrough for Report Submission


Upon extensively collecting data from various sources including explorers for CEX (Binance, Coinbase, Kucoin, Bybit, OKX) Hot Wallets and Gas suppliers, a straightforward Dune SQL query yielded approximately 3 million CEX deposit addresses (which are the addresses users send assets to for depositing into a CEX).

Once more utilizing the Dune Dashboard, I filtered out the CEX deposit addresses that had received funds from a minimum of 6 addresses regularly interacting with Layer Zero, leveraging an unofficial Dune Dashboard for this purpose.

A script utilized those 6-500 sized clusters of active Layer Zero addresses that shared the same CEX deposit address to amalgamate larger clusters. It achieved this by including addresses that interacted with the addresses of the cluster but not with the CEX deposit address. To minimize false positives, an address needed to be directly linked to at least 4 other addresses within the cluster to be included. Clusters with fewer than 20 addresses (21 including the CEX deposit address) were ultimately discarded.

This initial layer serves as the primary level of detection/proof. Each cluster comprises a substantial number of addresses sharing the same CEX deposit address, with each address being linked to at least 4 other addresses within the cluster. While this automated layer, driven by scripts, is slightly different from typical clusters due to the multiple interactions and the shared CEX deposit address, it still incurs a percentage of false positive addresses.

This is where the second layer of detection/proof proves invaluable. For each cluster outlined in this report, every address has undergone manual scrutiny, eliminating false positives and incorporating on-chain evidence into the cluster's description. These on-chain arguments serve as the second layer of detection/proof and encompass various forms: addresses within the cluster executing identical transactions simultaneously with identical amounts, a consistent transaction pattern for Layer Zero activities, and more. A multitude of resources were utilized, including LayerZero Scan, Dune, Debank, Arkham, Etherscan, and others, to ensure comprehensive analysis.

This entirely manual second layer, while not the most time-efficient approach, serves as a critical method to verify the sybil nature of the clusters and minimize the occurrence of false positives. Additionally, it demonstrates the extensive effort invested in analyzing each cluster thoroughly, reinforcing that the report is not merely a dump of a vast list of addresses.

The combination of these two layers, leveraging clusters based on shared CEX deposit addresses along with manually reported similar on-chain activities, constitutes a robust detection method with minimal false positives.

Activity preceding the snapshot was screened across 14 blockchains, with specific end blocks for each: Ethereum (end block 19757726), Optimism (end block 119326917), BSC (end block 38236464), Polygon (end block 56379454), Arbitrum (end block 205653169), Gnosis (end block 33677943), Linea (end block 4059728), Scroll (end block 5184468), Zksync (end block 32656745), Moonbeam (end block 6045324), Moonriver (end block 6637617), FTM (end block 80127182), Base (end block 13709885), and Celo (end block 25273962).

Furthermore, it's important to note that links on Arkham diagrams within this report are frequently missing, as Arkham only supports 7 out of the 14 mentioned blockchains.

# Reward Address (If Eligible)
0x7c66ea6c614c5f2f912c44825bb5aabc30b5b613

#Table of Contents

The subsequent section consolidates the rotation of the cluster's address list alongside its description, encompassing the shared CEX deposit address, an Arkham diagram, and the second layer of detection.

# Reported Addresses & Description

# CLUSTER 1

The first 6 addresses within the cluster are linked to the same Binance deposit address: 0xD6e68D8BD25FD515714BC934bE0D29051783bd5C. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.
```
0xd77a47c53bbc7f9afd96b1f4ca1ed7066961202a
0xffa009b0703ae2ad5d2bf4d0717971b1ac4f1c9d
0x6e70c39d396ecce2d26ede64b47860891310af4b
0x06890c8dbb688b500039c15b129bdab798b6dacd
0x6507a1b4736d56cb74e489087aa2cfb03eb70e62
0x387e4119f7d74de7e0065830e6c5002bf906dfbb

0x5f6a786b6da1d555030fd0f13222fc59f27c4cf9
0x2db78ad835e71dc0b4f18d80d0bd021e514c432e
0xdcc640b329555fc0a3e5c21b259627237e98d172

0xab56229144536ab044d93e8824d558223b9d372e
0x70af0e14b15b7699e789cb4ef50f4a8d16e9fe48

0x1413dc904bd949be7a2d46f12052f7674d7da1a5
0xbdfd420d70c3fb075908af9c7dba0d02ac8690ae
0xc836af736d276d44433d231b6114cedd77c585b8
0x274f5a0ce85e906456ef25e1f616132fd9ec377f
0xb0681de83f77c8374e9c8acf133f2271a93d6ec4
0xa2aa2ca76f06b4df26f3155722194ac6dad77025
0xbc8877ecae4b44e7d34e6c07b23112dd02f08b99
0xe17c8ddd7e4ea25adad2e4aa7cd4e1c83a5c84a1
```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/48214853-1bd5-41fc-aaf5-001762c17b16)

The addresses use the same applications: Syncswap is the one that comes back all the time with LPs of around 10 dollars, often made on the same dates. The first LZ txs were carried out each time within the same time frame (1 week max)

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/260e4d77-651a-4632-b0f6-6e54fc4a5e15)

Here we can see that the addresses made their first LZ transaction approximately 400 days ago, all on the same dates

![4](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/745ea92e-d0cc-4022-ab48-e00554652ea7)
![3](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/660df7d6-3b03-4879-8e4f-2b1a6f98f14d)
![2](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/bbb36e49-4265-4aa3-841c-d752cc3ba14e)
![1](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/abdd0a64-fe1b-40c9-a5cf-542169e4b743)
![5](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a2c1b2e1-c0fe-4b1e-8059-e0cd7587103d)

Here we can see from the layer zero scan the different addresses, the activity dates are similar, it also uses the same protocols each time. </details>





