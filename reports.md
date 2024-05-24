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

# CLUSTER 1

The first 17 addresses within the cluster are linked to the same Binance deposit address: 0x8968b4830D9bFDbd042474dEfFc0bBda731Db69B. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.
```
0x77c3db040f79ae46a91529a667c03ab484b37116
0x9d2e4bdc1e980e576a3a194f6f5eeda0ebd6dca1
0x61b482571b3ab0f74ccc8eee40fe4658b3ff50d3
0xebca8b5c9a3bdfb9ddf6be4ca807ad20fd5274e1
0x883a87de271a0f410351b62cda13e7e968011aaf
0x45233ff6bbc10f0eb41f430561ac97d78ddfb4cd
0x1626255e55b3c8fa14c933646534e9f8726c649a
0xfe8aa105f37c1ea271eab2fb698f752120bbfe08
0x54cf5fbd9a1ba2cbd23b321886d4848e3a0d47cf
0x512a3c8fb55c520f00dbe82133fa09de1c8d7bf9
0xd490d7ac76d1fe8ec0572c7f69ca4e99514c6164
0xd6f87ac3c02a65c4532c5231f66d78c3093d9622
0x302d8d638e10df112e705b3d9cfe33118e0e113d
0xdb0f1df85d3f3989c7543a8f74eb7d41132fe74a
0xf86aced730d6fa0340cd811f7b88adc13b22f5c2
0x18494636ed501765d3f9ad5795970717484b350c
0x2a2b5f1e522d18537e67a4b47aa31acdbd6be113
0x31c32051fca40b133cf9970cfaf141c11ec32512
0xe658fa69360a8351569fa79682f34f91d7a5c008
0x03fc17caaa63600351aaa4b736e8e2a901882931
0x790ea37af97f3b21bcfdc8d9ea8a1ed3ec05b6ef
0x331040149c9a5d5962659120ae57e8813426e683
0x5caeec615d50af25e2f626cea476bb0c2002a60b
0x584abc5b9434ec986529f77dba9ab7f58b415c8c
0xe74bc1aa5cb89c3fd6f66763fe433953bed19746
0x5d80de5c12858233d2e9a955c6604b6ce327dc32
0x8bade806405e01739b3c775061561290118b0af1
0x2ade36b300a279c89003a1dcf6378dd1d585bfb3
```

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ee6bc9ff-1852-415e-83d0-8a988cf8bff0)


I spotted this one on Dune, it was pretty easy given that he created and made his first transactions on several addresses on the same day 

And he repeated this several times, so I have several batches with different addresses in them.

<details>
  
![sybil1](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/772030b2-2c8c-4957-a728-cdc5adc07534)

As here we can see, its addresses were created on the same day, their first LZ tx was made on the same day, and this over several batches

 
I then went to check its addresses on LayerZero scan and we can see several patterns there

The best ranked addresses use the same applications: 
Stargate, Orderly, Superform and Holograph on approximately the same dates:

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5145e3d1-4186-4d0c-96c5-60d0ac740729)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/eb075290-d2af-4a48-85b2-c94a158e413e)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5ce4a15a-cdb9-45b5-a1e9-0c815a0e9b0c)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/aba5bad4-d717-450b-a867-7d9efc012f09)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a35f2167-182c-4523-b11f-24f64a7f9da7)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4f041720-016e-4730-997f-4f03df7d5a4f)

The smallest addresses also share the same patterns: We can start with the same number of messages, as well as the same applications used on almost the same dates

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/34355604-19ca-4b3b-980b-8dc06bcc51ad)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1aba5575-71fb-4743-b25c-3832d115c277)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/73c8ee18-50bf-479d-95f1-c9d9c6975bc2)

</details>

I think I have covered this sybil, I would like to clarify once again that all these addresses share the same unique Binance deposit address

From what I've seen, he uses several farming techniques, some with large wallets and others with smaller ones as reported.

# CLUSTER 3

The first 16 addresses within the cluster are linked to the same Binance deposit address: 0xAf25335F0290C8804a2357bc3Fd3879228FEd3f5. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0x14b35ea598a18e171a8f1e724c356f83fb4a0f18
0xd324c3e1da374f29077ca33d2e669456f897d80e
0x00a104b51215180cd87071962567cdff6961e0b7
0x7b6ac5df584f466fa8670b1107638dc7e940796f
0x4040ae6e1d67cc47060871ed9dd7c3eee7ad5284
0x98db5698bd3bbc83812d2a8e03e1411b847310ac
0x541bc299778baa8157a5bb093099791ff05b0cc4
0xb4d77e9a11425f8bb6924b374385282bf35a97d5
0xc8a60f7fc1ca1e2c1c13ee85ee1130024f69b07f
0xfcc49e880b3a024d2a31742178d86ca5cfe0169d
0x682463b16fcb871a17d4fb70a504fca7e4414b83
0x76cd684cb4b6148f667e6ee7896e2f6fcb3caa7e
0x106829fc39b9e826f694686b0211d54c710e3dea
0x129164e281f2e41a2bbdca56205c41649650a892
0xeb14da0a6f4260404fea6a596d3ae68599890f20
0x105d326450701879833e3cd33f161493f082902d
0x558fbb1b9dde11c85da59dee9b399bf37016a999
0xe5174798675530e1ccac4d121aa56d67c8b0bd3c
0x73f13a414d820b5e9118713c7466985890d2bbe8
0xc729d5a6eb0caaf27f4a68f31545ee88c252a0a1
0xb1a9c3c1841e55be6486d7844c2f8c791ea0d6d9
0xe719d984b5873ee40d4e81071b4cef7dceca48cc
0x692a15eab43e79f511abd4c26713c32301ec0252
```

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/48b8f4b1-db83-42d9-8a88-702cc3cf0852)

I spotted this one on Dune too, we can see that he first farmed with a main wallet then started making batches of addresses which also farmed

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6c1a31da-949a-43e9-bd9c-c4ce032a8c55)
As written above, he first farmed with a main wallet then made a batch of addresses on the same day, on different occasions

I noticed that it was a cluster following different transactions that it operates from several addresses on the same day, almost the same time.


![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/94abb163-0ac9-49eb-b77d-25b542b0d506) 


![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/36fd164c-e6e5-4eff-b1ea-bf72d2a828d5) 


![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5fe6fb4e-69a3-4a1d-8dff-b4f6c4f5a659) 


![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/58d1a0b3-39d7-40f8-a3df-4757d43faff8) 


![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/12b8f50b-ec5e-4f25-a333-d6ceeae58b9e) 


![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/19d3d6b9-8035-4440-a50d-a4d17deaf792) 


![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ee9e813d-d897-4414-a56c-a05dca23c053) 


![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/eb9ab7cf-d84d-4398-bc01-790e616dcdd2) 

The applications used are similar, but what appealed to me the most was the Aptos bridge with which it has the same volume on several addresses (around $2k)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a3be1803-1485-40aa-a617-7ae74c4d57d9)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2379c5b1-04d1-4bd4-ace2-ee07797761da)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/122569c9-5b3c-4954-aee9-2fdde2b45be8)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c93d1262-06cc-461f-8f85-ac7bdfe01a5a)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9ebc715f-cb72-46b3-a67e-eb0f0de87a06)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8dfb32ac-6736-4244-9f30-c960bf7c91c4)


![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/10955259-b38c-4445-90ec-fdeb73b47e13)


</details>

This one is obvious that it is a sybil, I remind you that all the addresses are linked and have interacted with the same Binance unique deposit address, which makes me even more confident about this report.

# CLUSTER 4

The first 18 addresses within the cluster are linked to the same Binance deposit address: 0xAf25335F0290C8804a2357bc3Fd3879228FEd3f5. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0xf55650e79a9945bcabb10953add13ff035d0dbfd
0x102008b16f49bc0f87427894012f0a616211d2a4
0x58c771b054edba5cf7d771c0291261ae50736513
0x082e4ac6f1bcfa6b31f4525fdfe30c685df759ed
0x89ed5d9f29789c0c55f415bbcd2ba259882307c0
0x09774238fd4a4569b9319743a80e95f18f41e4e1
0xb23ec4fb34479b2024597f7681d6cde923dfe916
0x0a389c8c7101409831e81c82dcc9cdb13dfb4e39
0x7c5829dfdfb607328824475e98612e1e8862d3f4
0x815611ea3f076c2f0d5e5742431ef16cca577967
0xcbba4a3ab07e76b57fd53e46f6ffd8dea5dced1b
0xb1fba78da54ea383d3558f458d9cfc75b656111e
0x9d37e8c4b4263093d812f7382c659e05c34d7ed4
0x9daaa0ff2be321b03b78165f5ad21a44e3c14bd6
0x763d03f7458e68dbebe324748a5065c316e4b155
0xd87f4e2fa65daad33c413ea5bdbd8c0b1c4358a8
0x0cf1368538c7f7994259428081d7f86f3ddd5545
0x33f50b61c2e622494cb9906cc42eaa0675707781
0x88483f6ac6a29d6314fada20881af919a13f6a9b
0x5b68f545836991354dd6408d28bde37584bc69eb
0x9990f9aad45563e2e81abad122ea790d4f4050fa
```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d153cd39-ec5c-464f-bf39-7ecee768cab7)

This one was more complicated given that he has SEVERAL very high rank addresses with whom he is careful not to get sybil

Unfortunately for him I managed to connect several pieces of information proving that he is indeed a sybil

<details>

Let's start on Dune, it has several addy having their first tx on Layer Zero on the same day and who have roughly the same number of transactions for some

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/eacc2cec-f402-4fa6-9a8b-f23efcae790f)


Then come to the most interesting part, we can see that he carried out the same transactions, at the same times and with several different addresses (especially the best ranked ones)
</details>

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/451763fa-dbcb-4263-af0d-e823c0cb61b0)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5054fea2-61e2-451a-b152-67dbac733575)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2bfb9845-e574-48f3-b70b-1a01a131a649)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/642b4d5f-dde9-462e-861f-aa696e84d27a)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1d165ea9-857d-4bb0-8bb5-2815e7efe464)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/334781b6-7e13-49c4-ad1a-73e925b78ff6)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/90ed7775-813b-426d-8141-274044aa75b4)

Here we can see that he executes the same transactions, at the same times, I am sure that it is a sybil even if these transactions are not carried out on Layer Zero, we can see that it is the same person behind

Furthermore, if we look at his following and followers on Debank, we can see that most of the addresses are followed by the same address: 

0x73e616b9e20789c5e0102ad7c0bc8bec42dc6a58

I also noticed that he used Orderly on the same day on several different addresses, I will then list the TX according to the dates used (which are the same, I remind again that all the addresses are linked to the same Binance unique deposit address)

11 APRIL between Most of it happens between 11:00 and 12:00 GMT
https://layerzeroscan.com/tx/0xc4d2261d5b5525ca38e1dd6f3431f3fe97e78e07c739be1a577204f476dace73
https://layerzeroscan.com/tx/0x3a53dc700c26ad34db287a328d506febe5803fff40dea595b07370a0ee76a5e1
https://layerzeroscan.com/tx/0x8d8ca07f34bd07780d346e5e3feb164865c230ae1c9110f37fe43ad91707483a
https://layerzeroscan.com/tx/0xc4d2261d5b5525ca38e1dd6f3431f3fe97e78e07c739be1a577204f476dace73
https://layerzeroscan.com/tx/0x2592b5e3d5a570e804d67273404bc1f2da5ccd26ed49ee33fd177718a3ce6f1e
https://layerzeroscan.com/tx/0xa9e5809f1368bc15a2f3bbf0e063ec975cd3906005e722da1bfbec5c08d2f26f

14 APRIL Most of it happens between 9:50 and 12:00. GMT
https://layerzeroscan.com/tx/0xe6bacaa3c1d68bff4e83b1d8fc85efcef42a600c839965801b7f1b667ed4e019
https://layerzeroscan.com/tx/0xadbdc6b504c81db57be01a0d9195312d4fc0280495bdbc6d1ab1ef936223e24f
https://layerzeroscan.com/tx/0x1316c013733cfcfdaa27751e2aa33465c840eec85b784e49dd9388a2567c5450
https://layerzeroscan.com/tx/0x15e91b65ac790d6915190a3e44898e7759f3aa51ba85159f7a7d9221b52294cb
https://layerzeroscan.com/tx/0xdf470193bbfb4b2c3ccb2392323a8fb1021f520da5b0ef57e73ba76bc7bd4c47
https://layerzeroscan.com/tx/0xe5f712a3cad67f305e971315f5d48d10c84bacd4d0e0a6f0ff1bdb8a5c8a805d
https://layerzeroscan.com/tx/0xb946f269f5af3cdab2f0f0498576e7ccb105f2f7531179e47ae2d9d7ac780782

14 APRIL Most of it happens between 9:50 and 12:00. GMT, some are after
https://layerzeroscan.com/tx/0xdeea92353e4ad958a34e0fd45d9eda95208d9a93d18f343efcc781cef0871b6c
https://layerzeroscan.com/tx/0xba24d767afd2c185f01e04d24d31a96a0d9614dd049d5b3fcba7b38fdc060d28
https://layerzeroscan.com/tx/0x6f0dc1f0ed3b360825cd25fede5e04c386d6b430e9d12be639b2d00b7af9010c
https://layerzeroscan.com/tx/0x6126a505e090fcc5b13ccaa11305455dffacb887436e8d815b30eb071a3ef72a
https://layerzeroscan.com/tx/0xba24d767afd2c185f01e04d24d31a96a0d9614dd049d5b3fcba7b38fdc060d28
https://layerzeroscan.com/tx/0xd8e4ef21efef1a32670133a146ba79271123d8d9147527380d1ea8e72f06bd3b
https://layerzeroscan.com/tx/0x1d101c450f1c92d9609c78be3ad058b4e415c3fa0f6d6a9d0d6abf8cde8c9362

</details>











