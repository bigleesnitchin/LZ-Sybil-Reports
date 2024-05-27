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

# CLUSTER 2

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

This cluster was harder to dissect but as indicated, I managed to connect several addresses which carried out the same transactions
As written earlier, this one has a lot of addresses, some are very well ranked with a large number of transactions

What betrays this cluster are the addresses that it created at the same time later to farm

Unfortunately, he uses the same applications at the same times for his well-ranked addresses as for batch of addresses created later.


# CLUSTER 5

The first 18 addresses within the cluster are linked to the same Binance deposit address: 0x4B505Cd61AfDA49F231726271c84627B2666F809. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0x63c24f164fa69f4db7f45f211a8e089c157b4747
0x6e2ce22c13eff481456db5c975fdd0e3f161f611
0x4e91394b30162d5a63a09f5cfe253a09d05254c5
0xbcc543e49afbaecfb65f4cdbeac271a97e735f45
0x3d8b8ea64af099a0d2dfd9f0c97164628ee422e7
0x53157a5ff07955f323a7624ae81c1add7e15d9fc
0xa4bd43301b38698faac1a179f2d2729e2ebb2dfd
0x427da433d001c8e4e4991a544575dafaf493399d
0xcdac5fa9d6f811a1e63714b0d4fe7bbebe07df0b
0x695aa322e8b30aef3a0a417bd49612fc69b9313f
0x64ea7be4d6ed0621aefe1ffe6d7d38e9a6396eb7
0x2c3d78b8ab518d5ff6b909343f6865df41b3dcf0
0xc1e66188827800152f5e98190f9c59c9ecbcfed0
0x45f93ad7124ddd2d578e40de6f0836548433707c
0xa872e46e6da69402303522bcdf9f4538d16175ed
0xc9f308d054b9c66a65dbcc1878772707ba96135e
0x600d1bf9ad00514196ed9a96c5afbddb471478c9
0x8d1d836f06d271028d028b4fb7ba4386795b9d0d
0xca8ba91243bee135fdf59fc509b27fded695c387
0x6216977058c2a6ce9b910a119f3d0131b0e7889d
0xc60b220f62578df2e584349dfb3a771780a300ed
0x327a8065328da20491ff01a7735733c8c39bb685
```

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a338e2d8-c357-4de6-a839-934f1ed64878)

This one was pretty easy to find, he made several batches of addresses which carried out their first transaction on the same day (cf Dune s/s)

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8449df58-f04c-4973-91be-e7f8366dd50b)
As you can see, he created his batch of addresses each time on the same day. Then he made his first Layer Zero trades on the same day as well
We can also see that he has approximately the same number of transactions on the address batches
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/dc444327-3b5d-4ebf-a242-1c68a7c55ef9)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5bcc4325-c7e5-4d0d-b21a-192c0b723832)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/323e1639-102e-49d1-bd3c-7f02ac2ec922)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2bc0aaa4-dea7-47fd-835e-9a5fd39dec28)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f1e04b18-dfbe-4c7a-bf15-16e28b3c3143)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/db25f003-a134-4f56-bc8f-0749b517575a)
</details>

This one is a sybil for sure, just on the dates of creation of wallet it helped me to know but to be sure I checked several of his addresses and I noticed that he made the same transaction on Syncswap the same day.

In addition to that it almost only uses Syncswap on all wallets.

# CLUSTER 6
The first 18 addresses within the cluster are linked to the same Binance deposit address: 0xC4B9687ED789FA9Fee96d2BD880CC904c78163a1. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0xb09110e39e0db45dfd7797109882014e7a66038b
0x0283a23b62fcb3e37fcd4205d499ae42bfc4340a
0xf3443f7071a4b39908acabc6bff79cf64296d235
0x12889eba53806e26c663bbd5f3779baedaaf2822
0x650849425bb8401f08e217dbf7ca22f753e25744
0x90d107b34e84ae88b57b54f095f090252280dc2a
0x1e82cdc70375fff785b695b38976b83b79a30c2f
0xf37a48956560079dde12159a47935f2d5e9169fb
0x57d1d4dc4e3f05f68ffe78d61193558e0ec71961
0x372fa25ea9647da526b5b001bd18361f00f2d408
0xee9b89df4d6565a7c22b0787db62e00b0df1f6c7
0x3f17ef1accd9c705030ea6ea72d7a64554ff5220
0x59e133b2114289f7b506e13e7f86c694e1b94734
0xd02691f93ac36db3038a4159bd2ac24bef39d360
0xfbb16d668e9b83e677d6170eb977dbe3165bff3e
0x7e68a7a2ade5b537b907fa9d1943ad70c915ec86
0x0b95f218d9032ebcb9ea928c7621e2ec7d19e390
0x8434f6eae6c543ca61bf94e4b3d797a99afc008e
0x4edc30792623c82b02d9ce770ba9b32ea68f4244
0x70c993f4f788554dcb2f6762a50230eeeee71636
0xb9c4b3ff78912051f0c92155e15c82391619f39f
0xd932e0c681d182cd576f6df450c716c7dfc89956
0x5cfcaee09dac4c664b948ad7dec41d5554afd043
0x7a19c1948df3153aed47da5a3606a531d775b8cd
0x7ac9e6dd61a4ac8f9cd3ed3a52100c3f54bef57c
0xecec188d4299d8f00d8942f9b2e9b7210e9bb614
0x625ef20d6b8594213ca014f1009d137c90fececd
```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/679e3239-894b-4e6a-95b3-0f81180c2701)

This one was a little harder to find since the addresses were created on different days and didn't have the same number of transactions, I had to look for more evidence directly on chain

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0ff6ddde-71f6-44fb-b067-9a30dc412689)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3557b942-d465-4bc7-a748-c449c800b721)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0f85849c-ffd7-44b5-9888-66c537c0eb25)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/7150d87e-0077-424f-a2f8-c34cc7cb9887)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/96a9a674-f862-4d38-917b-b21791faa962)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/7c48af70-9843-40fd-8021-af20366b222f)
We can see that different of his wallets had a lot of activity between the evening of 05/18/23 and 05/19/23, all on SyncSwap

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d3e6b34c-0859-498e-99b6-11e20e4852ee)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/aec3de6a-afb7-4f6b-a039-a9fdf6d71fbd)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ab039198-8908-43c4-a8ba-e49be42db69a)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e8168bc2-2512-40af-ae39-9fca402e9ceb)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/775e9383-845f-45f8-b675-b01ce40b5a14)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9cfd8f57-cb84-4857-9ac4-403214e99da2)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8ebcd5a0-1445-4bab-8840-61a4165319c8)

We can also see that SyncSwap is its top protocol on its top addresses, it comes back every time.
I remind you that all these addresses share the same/interacted with the same unique Binance deposit address
</details>

This one was a little more difficult since there wasn't much evidence on Dune, I had to manage on chain but like all sybils it makes mistakes, in this case it frequently uses SyncSwap on his addresses, I was able to find a day when he made transactions on quite a few of his addresses.

# CLUSTER 7
The first 19 addresses within the cluster are linked to the same Binance deposit address: 0x127e32704c645a00E56CEaa78A6E973A14511dB8. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.
```
0x0125054443c774ac1009187b54bd6b035ee4c61a
0x30dddde80843855ea3d7570c11a5c993365e5b20
0x400996bc4bf162ef75dde4e7a5d96c7e4d0e3e57
0x7c5c6f2970e6d50a48f3f99a213335f61c8a2d4a
0x49a52656696b97d5a2363db0d05c4b0da1453f2a
0x27ece28bfbf510ac79e0422bad99bc45058b08a3
0xa00acb286bf2c21a1360ecc48ad0c961916508d0
0x9b5a5580183a96e090210b48ef86bf97eb3724fd
0x2cf3ff760cfdefe248f53a12dfca2ee887d27637
0x1435109a44fc9e054d2f0c8c7a46656f1bd1d9af
0x987c15e6c547b0c1cd434308dc53225e503f101c
0x2826a704404a44a951f892d17af4e409dc0e6218
0x06eb75c251183dbf6e33df96e93f7d04556790d6
0x8e445245b2301762e850606cf8767e80915231e1
0x3ae627abfef7d41a7c2c0ec1df3e0ddcb3b621df
0xf94d545f8c0154cb7cad6fcf2cbd494371f36fd5
0x0a2f025dca948bda7eef9f2d10a5b0b864c1fccf
0xbe6bd50565199c4eab3bca7b96d3a8331f06dfea
0x4eb62eee2b9911b24208552628c009b2f44f0c7c
0xff05cb914b4b6b25fd82100e2503e37923590063
0x175a0cc46a5430c62f48368f5cba1c66b4b3d56d

```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ad21694e-467e-433c-9a26-bdbbf3b54dd5)

This one is one of my favorite types of sybil, he made batches of addresses having had their first LZ interaction on the same day that I found on Dune

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/587d4c23-8f4c-4a56-a2d1-6da152b15203)
Here it's not difficult to spot, he made his first TXs the same day on a batch of addresses
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/fea21bc2-c6a2-4b69-869d-3c9ebfe4c1f5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b8d69321-0538-4cf8-aaf2-97d38f3813ab)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a9932b3f-18f9-47db-a77a-9a617ac15506)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/99c11866-d9ba-4f04-b6e1-fc1bc9729c1e)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f1c06030-1e3b-436a-afff-5c30ef636536)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/aa6a709c-9bc8-484e-aade-fa9bdb75c1e3)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/20a01bf5-9b87-402b-8a48-cc9fb5e8eb52)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1ab13910-ecb9-4bcd-a354-c373ae18d4f9)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/bf1bbc18-c0fc-409f-bb85-b9996ced3e49)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8682da42-af37-47e8-a160-5bd93a190af5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1f2cbd20-176f-4728-a3ec-bea3dd12d730)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a920a323-4a69-4767-851d-f5676ac8b142)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/82298520-916a-43f8-9b99-8c492948fd77)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6e45e110-6720-4648-a9b4-7e1997cacf24)
He also used the arbitrum bridge on the same day on several addresses on the list

Here we can see that he farmed another airdrop two years ago, he used the Optimism bridge on several addresses on 04/12/22
</details>

Classic Sybil which makes batches of addresses which have already interacted with each other as well as with the same Binance deposit address. (Like all other clusters)

# CLUSTER 8

The first 19 addresses within the cluster are linked to the same Binance deposit address: 0x321cBAdB105aB951Aa2Ff015cB268db641568a63. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.
```
0xc89bd5d46d4ccda62207bedbb15b6b28641c4277
0x96c019c06f59be7681bac7da25bea92820299e2c
0x47207bdb6f6475ef07dee363dbab9b09d891323f
0xb5b2b10d4d15fd54446e202ab6f18af575d28390
0xed8257292b822cfc513c450b736ca2769aef7267
0x7bf06a0967b642b2742a73a9a91ce8bf18b7c3ef
0xde890a6de9b4c65a0aa51280bf142528a2059e74
0x7b0ae6b1fdb107da2b9259d7bfd4e3fe4eeae858
0xf96b9e7818a63e2510278240200b0aabae32eb32
0xa024e85ea6b0c6e3733909d258783672df0c7668
0x819b6ad8340f694f13c741655e749366e5fdc750
0x574eed1d8b45077b6513ee9e433fb104a1a99047
0xec1e8b34fd51a53f1e44f40a31a6a6428f2529bb
0xd91906202dbfa4e9182e2ff3549e2023fe7c69a4
0x305edf50c41ec022d7def07cbc6b78ab7c9e25da
0xe1ef9f054ff7dc129775f7a38720b257f7efe417
0xb44f6554eb9c6da5e7fb776cfde031da724887e1
0xb2dc8730944e592f73d8379e00c973ae165190c9
0x8808b966f5e84b920aa354221c469a8f47886646
0xc30e37b20ff172b235f9b10bb367ddc257b55d5e

```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/881ddaa1-dac9-4c7b-a8b4-75b152dd9889)


Another one who made batches of addresses, I will add some proofs on chain to be sure.

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/83b34fb8-22a0-4eb1-9c25-3dbd82513b4c)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ce9db298-ba27-46e4-a507-b44cbc58d863)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e6cb9dcd-383f-4c08-80db-211c56ad6855)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2bd6c885-748c-4234-a1f4-9dc7e3d0c6d7)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/770987f2-b3a3-419c-ba70-9ffff34cb51c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/fa43ee57-fff9-4348-9f2e-9f17e9181ef2)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e2feb7ce-1fa0-402f-a3fb-31cd4702907f)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/50e8988b-217d-4bb9-ac85-10eb2813a5df)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/82db7a8b-ce37-44ad-8bad-1cf7d8bb254a)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/043a7876-c773-4f51-afa5-a072edddea11)
Here we can see that he reproduced the same tx, the same day on several addresses
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8075e7c0-9e23-4cf2-8f45-1eb9261243bc)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9ef1b326-2771-4eeb-a467-b5d56d4c09d4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9fc167fa-6427-4deb-b7f3-dc328dd07f56)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0b878f2c-4149-4133-97cb-3e01a58157e5)
Here we can see that he added liquidity on the same day several times on other different addresses again
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9bd6030a-e69f-4237-b6e7-8e7fde22a4cb)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d8bb9bd0-4383-4873-a716-4d851c37c0e3)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6f287b3d-6f61-4891-a3fc-70cb632d96dc)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2f7e3ebd-140c-4005-b4fc-27e4bc4475fc)









</details>

This one was a rather easy sybil to prove, it reproduces the same transactions on Stargate Arbitrum

Bonus: We can see that he mainly uses Stargate on several chains with all the addresses to make volume, I suspect scripting on that one. I only put a few screens but absolutely all of his addresses make up a huge volume on Stargate. 

# CLUSTER 9

The first 13 addresses within the cluster are linked to the same Binance deposit address: 0xFb1C9582d64f31c546Eac2a1d8f4c00DcBC03262. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.
```
0xa1b0d7162a63457bb2bc0a8825c5fac48dd92c25
0xba9f9664571d41ed2d9486cbf64bedd399979a50
0xa9512bbdd38cbc1041ca167c55664c421ba77fb0
0xc96b4f52ca0f9a49dfd7fcaa6edcae9bd3053d09
0xfbb3351c603db8ffc9e8d683a930bb3f8d85eaea
0xcc8649e011f0c50892edfc72c4cbb2dd350295df
0xc4838ae9f077652792e462def589237a6d97d47e
0x4174568edeac7e38fe86c115a2a1434c51564c4e
0xaa43f62d03990bc39abbdb0874269152a186101f
0x11f64d387663f91499b38e539390b9aafa372cf3
0x79799ed6c3146dd4079f69936461e3d01df84d95
0x03fbbd22ea24faa2217d669b142e1ad38be4eee8
0x0c38f5018ad634aebc2ae514d1e6ce42992f4931
0x809ab464e2c313b4806d700c7e37233f5e01e48c
0x80ead9c9ea42c71c27a6d8c403d9b81640f5db91
0x5b57abcf3d3efabe9d4cf0a280c42e8403d1ae49
0xf60db0135520d634892c102f7d59b7e21557c4d7
0x653871118edbe7d8666b9fa6937d0e9b24ae29ee
0x52942386567728cd1c8ba1fd430561781e121f1e
0xe5223b9d911d3cf795ba498bde288dedd62eeac7
0x98d52aaa2b4342306876de1402711fffca1bccce
0xaa878d5b057beabe4192f85391553c6da00c92c0
0x38214aee1e548dda463e6ead4db91044f76a0657
0x174d3739438b87eecb86e5dca163ba0032221556
0x773d1df6da28ce91b9c877d52ee88be8cef2b956
0x757b421e5c49f7666dfe44be04228b8881341245
0x1b52bf8ec3e5260e82e8841f878244239b50bd86
0x11e3472d4a3ce3d2afad277af5d096946d145b2a
0x8e32c75f65b7a7d6c6b571ff078217e930436881
0x388fe51c388176d269309226893fdd6f5cf3a517
```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8d7712d6-dea5-4fcf-a603-51c99747607e)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/723e3a64-b80b-4e46-88d1-3654755bd381)

He created 35 addresses in 10 days and started farming, I will bring some arguments on chain in addition.

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e9b0f868-a815-4d52-abfa-2780a0a9ef7c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/31c714e8-ba71-4ff0-9e4c-0240d8f785cf)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f048d641-45ce-4ab9-8da2-094754a5fd1a)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3dcd09a1-327a-401f-92fa-af6fbad244e1)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4d6507a2-0eec-4f3b-9044-e585fe8e64f3)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/af1278b3-efd6-4b48-94e9-91e2b4935633)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d40aad84-bc7b-4a88-b0ed-3fc0bf4e169c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f76fc268-e828-4450-a73a-1012dbf90beb)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d23a8014-a185-47c0-ae6b-c1b5efdf211e)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/68125de8-ffdb-4715-8588-d0872fce3982)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1d55341b-0a32-43f5-b055-c9035c6a7180)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/7ca1ad02-d1cb-4412-8963-7e2ade4a1ce4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b86bd515-e0c0-495e-b738-06c03dba0324)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d724b6c9-4f19-45ef-9956-f28de41b54c8)

. ```Ok here we can see that he's only using the same chain to bridge his funds and make volume with ALL HIS WALLET litterrally. 
We can also notice that he sends funds to the same address that we find each time on the screens: 
0x80c67432656d59144ceff962e8faf8926599bcf8
This address is the Orbiter Bridge. ```

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/7a8064ae-8c69-493d-bc2f-6e4c68c722aa)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/da8752f9-f5ff-479f-8711-56f1cc63fbb2)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1c01d9d0-c94f-45ab-8ccf-da2c071b7da2)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/cf415120-8c18-4786-9d56-515ad1c5e39a)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/844b4979-48da-42c6-aa55-78e717978e86)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/50a8ae36-90fc-4110-b18e-126ce3875782)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f9b4ade6-c80f-4918-948e-97c637ca1959)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3e2b2572-d5da-4b71-99f3-db9152c8e8bc)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a5f3214c-4456-406f-9419-64a479ffb939)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c5ac0dab-f7d8-4d0e-84f0-58503e17a5cf)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b7985178-66be-4735-a7a9-937eea43ef3d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5a4fb7d9-6882-4ed1-943f-8991fde97da2)

``` He make the same transactions, the same day on all addresses ```
</details> 
As we can see on the screens, all its addresses produce the same transactions.
This one is a big compulsive farmer, easy to find from the Dune data. 
He produces volume by bridging from Avalanche to Arbitrum and so on with all his wallets.


# CLUSTER 10

The first 34 addresses within the cluster are linked to the same Binance deposit address: 0x857Ed5fabd064aB4849Ff45e5d6d216B8D5C4722. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.
```
0x0de40f29e25a84f930ba94c7c5972ac865d2e664
0xede3111ecb55b66abf6a20bb543d2dea8720b0f9
0xf1e23eed94ae3506186957b91936417c6ea616f5
0xcfd513ed7fcde1d2fd4fddfdaec1b649bbfe32cd
0xd3e0c5608425381fc26a126d56925d3165e5162f
0xdcce380a82250594f4196573af4632ac57cc05c7
0x61b4acab4a1da4776fe128833ff321aef9e1cca5
0x80c6108a451d09a7e49b2ce021dcedf8ea538b56
0x4c3d9d0396e416237cb043365c0b33c0fe23ffe8
0x95237518bd575d83c0caa42b9d2a6885b7a3281e
0x573f9a25213eb34c3edfb2c6a160269bfa211238
0xa4f26389dee3f7e9ee635a3f75ee5cf1e7bc7504
0x952d90403d485d2c1cd9477dfcd64278b1979c0b
0xee53545f4a8e0142996ee4eb214d3958ccaed6a0
0x16ee72279d51c8672617fa85da2dcee9da3dcb86
0xcfbbafd932a7fbfb951c2c3e8620d6b64b6a1813
0x22febcb64f8bb2291174185bd3d29ff0cacb2c8e
0x34f5dd309308377f405a88af090c696e506b60e0
0x9c2e7e0fa8ad2b24e2dcd7291f65a46fe184180d
0x19df559bf6c57579c5c7b32faeaa46f35cca5a79
0x8e57efbea55b77a3336256b2f1525773a7c87ca9
0xda22bd2188c9ea594bd6f06689a93ea6c55d1ef1
0x1b550e4ef8e5358e4527337d94c7e9b1eb953e58
0x434c83625c0e4762f695f6084b924bde365382a3
0x93eb20245a21be03741212eb6cae1fd00698f297
0xe84172a861d0862855a75c21bec5afbe4cbce119
0xee9c6674877d840fd9b5093f84f45b7e2c3103f1
0x5d90df94547a3442f2f27f0349908889fac95d7c
0x13b0c3f89f70f9bfd0b4f5d399b4368f7d86b919
0xbb512125590566686a9c6cbd13efd70eab15bdb2
0xb16eff06d5e59f2628ab264c0c2f2aa91f5660c8
0x0de40f29e25a84f930ba94c7c5972ac865d2e664
0x59604bee5568e13a00d7dc92ebf78d368a22e226
0xbd9225654f5ab656482b9612420c0c6cb973a7f8
0xd9f82e69beb23fa5ae199435cbae24da29d6a4cd
0x0b10a4dfae294b3e260d97c92b3588790fcb40f5
0x825fcf392b10798b90d2fc819f266eb1b1eacf15
0x915e483b6efc2e4ff3e2f1379a5d8c5e8c9a4f8f
0x333df78653f266d88679150ec62530a522d71ed3
0xb6cb72715384d86286443eef5d48e98b144a7ef8
0x6458b344429d2c79bd7c78a3ada2db749cb36b3a
0xc8fb30a884a9c9533844aa5ef7576226235a5f9e
0x915e483b6efc2e4ff3e2f1379a5d8c5e8c9a4f8f
0x6e257ee90b29df336d962a2f7284568abef92b6f
0xa6ca777daa600c0b4325f0ba038b34fb008fc0c0
0x8afa1b7aff5398fca53129b7c980a35b2fc1f677
0x5d90df94547a3442f2f27f0349908889fac95d7c
0x0de40f29e25a84f930ba94c7c5972ac865d2e664
0xede3111ecb55b66abf6a20bb543d2dea8720b0f9
0xf1e23eed94ae3506186957b91936417c6ea616f5
0xcfd513ed7fcde1d2fd4fddfdaec1b649bbfe32cd
0xd3e0c5608425381fc26a126d56925d3165e5162f
0xdcce380a82250594f4196573af4632ac57cc05c7
0x61b4acab4a1da4776fe128833ff321aef9e1cca5
```

<img width="689" alt="Capture d’écran 2024-05-26 à 14 24 39" src="https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c3facd92-9e36-4be6-a124-289e667bf306">


This one is one of the biggest sybils, I even suspect a script behind it, it was rather easy to find and farm with around thirty addresses if not more. 

<details>
<img width="1185" alt="Capture d’écran 2024-05-26 à 14 30 54" src="https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a989ba34-2ad1-4093-81c6-fc1f51178c40">
<img width="1202" alt="Capture d’écran 2024-05-26 à 14 31 25" src="https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/58cb8cb9-6486-4d8b-b4cb-e5c77f49dd44">
As we can see, the wallets were created and made their first TX LZ on the same day, this is one of the easiest sybil patterns to spot

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f7e12e8c-d2a8-4326-b538-8600bb2a5218)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f31e5abc-0862-4864-b5e8-941b02e13350)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4366e078-bdad-4011-a80b-4225799d3d6d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/53fd2720-95d8-495a-844f-dd18190cccc8)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/fa25f090-22c9-41c0-8b38-969725795f9c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ca5ea213-046d-4a92-8272-d6bf9b797d0e)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a063fd35-414b-45d0-a679-9860a52285f8)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e1d7e10f-2cc9-4240-9556-839832616d1f)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8b660c2b-1d3d-43da-a5de-05b8c392e885)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/26f72d6d-69ae-46e4-92dd-dd890182edb1)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2678aa98-18dc-40f8-b657-0adb19f39900)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4af61347-00b4-4998-8ee0-427e2de897cc)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0441102e-6c3b-4562-b717-09ff85c9631c)


Here we can see that on 07/05 he sent about 0.55 Avax then started to do volume with decent amounts, he has over $1 million in volume on Hashflow with several addresses on Avalanche.
He made over $10m in volume on several addresses 
on the Arbitrum network.
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/91a893e4-b6e1-4d67-ab72-092e44ec95d9)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d5287a74-68da-492a-ac8e-66f43001cdba)
Same TX again on other addresses
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5f8ebfe0-6b6c-4b37-881c-b2da87894b98)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/fb95c5f1-59f2-4c33-841b-a9b01a817808)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/56d4eb21-405c-4717-b8a5-430bafd52bfb)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b8b83e03-2477-47aa-9efb-4eed76567258)
Same farming TX on Maverick, its goal is clearly to generate volume

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/209a1892-b44d-4eb5-96c4-37b9674a2dc1)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/bc0e976f-8a32-4058-8459-4bc02fd76eb8)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b1069017-16bd-4d24-bfb4-e35518d097f5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/470edb35-f45f-4579-a488-bcf26d1c5797)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1ae1465c-cb93-4fe2-9c45-4e5e29278fd1)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/597625a5-93ed-4d13-847a-4d25bb18c716)

Same farming TX on Kinza Finance, its goal is clearly to generate volume

</details>
This one was a big Sybil with a lot of addresses that farmed mainly Hashflow, I traced it from there.
He has quite a bit of volume on the protocol.


# CLUSTER 11

The first 19 addresses within the cluster are linked to the same OKX Wallet deposit address: 0xC5613681D7620a8669b81fb29a96afDC57D5A068. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.
```
0x637fdcb9502384869d35ef528f977f5bf885e639
0x558b2014ee4897ee2cc68c6ff925935f7b1bca98
0xc0e769c29c75b7a414e1fc3e14c2fd13bc1fee0c
0x0bcf2a009115e033095de5499520b4a99d1e212c
0x27c9f8f3b6736b2b908be59c8281c3af0a139621
0x3424f6691797956bb2a495244e82e6f2c1167645
0xe9cbba76935e379fac350c18e9218f8335f1b161
0x3a460dbb24d7187d6260ec22362baab696db5d24
0x37ef45a1148e4eb64c9d5a5f65c403a400d64781
0xd2601febf597cad7cfc573e92124d263c369d48e
0x6e48536eaf5a16e99486bba2ecf7ecd457be58ad
0xdd531b9ca5bcbe81c40098f56268ebefdccd8760
0x0d9c95b4c7fc61d25d1e450e32f8d0b1fb8abb37
0xeaf72c8a245185f289c870870397d81e5dfa2c68
0x9cf161127f3e0d9406f2e48c8252500e9cffda61
0x4fb0c65c0b412bcd19f6047eaa35c333c5bfa86a
0x2e30a17929f173f80218fe75096f625edad08b8e
0x8ccfaa9d8f2b34ae525d202d65712fca81da4cea
0x0710e1ebebb584425ebf231fb1aa875f5b8aee52
0x2d5abc8edcd5c6f6ec419a223ba724558d6122bb
0x8dcfb6cb50d98aeb47d30e90181bc7d0f5512b41
0xb5bd472975dd3e335541d84c0790cb836a70b7a4
0x280b4c58dcf404d76961f57a7a781744fb38722a
```
<img width="655" alt="Capture d’écran 2024-05-26 à 15 24 05" src="https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1d723ad7-faec-4af3-8bfc-47c64d58193a">

I spotted this one from Dune. I saw that he made several batches of addresses with whom he made his first TX LZ on the same day.

<details>
<img width="1372" alt="Capture d’écran 2024-05-26 à 15 26 37" src="https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/812699de-18fa-4355-baa2-9e1002593adf">
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/01efeedb-3526-4c99-9e5a-a497f8a6fab2)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e617b0b0-a89f-46ad-9228-2121f6832010)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8b3f8bfa-1c55-492c-8dca-0a9609965aff)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f9dde1c7-3765-44ea-8faf-872c5b1f048d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/88d1b8a6-133c-48ff-8b81-43000f129140)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/99846c9b-110e-4a00-b59f-90d5178b881d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/26f43171-5cfd-4e84-9d78-98b9ec73663e)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/bd84b4df-e95c-4757-9212-08cb5a7bf5b5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2be2d0b1-0641-4b3c-bb42-9ed0b8ff7342)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/25904c3c-94de-41d4-850b-7654ca688e78)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2aa52db4-db40-437c-b129-253dbbbc5588)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/902ab531-a63b-4929-a3c4-8df9f1ec2ff8)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a5a80cac-e08d-4761-a222-6d1065268e57)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c952026d-4cdc-48ec-bebc-e39d06b57ef3)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b82cfab9-6683-40ed-9235-8c265e43e2a8)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6e12224e-a9ed-4c71-8a9c-f1f2da654459)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/da74051a-ae4a-476d-9417-80d73b33fbf3)

# Between 05/13 and 05/14 he did approximately the same volume on Stargate (Arbitrum chain) with his batch of addresses, the same on 08/22 I put the screens below

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/cdd31758-2703-4789-8ff7-333030d87457)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/eae89f4c-7355-4080-a026-1df7ebd28665)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/cbd06bb8-b4c2-40b1-8955-092ac2fe4365)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b2c2a9b7-b53f-4dd3-b579-b55947d4c403)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/17626361-93c6-429b-a6c5-f8d30896ccc8)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4074acc9-ff28-4658-a674-0265697c6d6b)



  
</details>

An obvious Sybil, maybe even a script given the number of wallets, in any case that makes one less.



# CLUSTER 12

The first 5 addresses within the cluster are linked to the same OKX deposit address: 0xaAecAce720A40Ef21d0545efeb1bd965B67DE1B6. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.
```
0xe356e7af80b8626a2b6ec11c32ad936c50a98a92
0xd4f20f43eef492a6cb117c698c0a1cbba42811e4
0x247119d2fe1e1276341b39235dafaf48901603fe
0x653b4c9532363bb07d36d93820e6916c17663bae
0x90208ffbf774d70b1433f6d64709fdf62104f77a
0xd2033db9c5370ac76abd80823b5c5adc097e2fbf
0xc5840af43749fd2a85103165c88e1891d2a64582
0xccbc524ebe1a9d7f0db3fbd10bc5c6e57768a28e
0xb2dd985116db690461fa28e03ba2a08a60af90a1
0x4bdcba858dca35ecdc2a61bf0db4780e19a2d7dd
0x5c29e2143a07f0b20a5881e1a353f95140c73d83
0x5c33052e154964da3d26c8b8610d508df050476e
0x645237614d9472698c225d19acfe447b039fe4d7
0xacc00e45cfe70154c9e058e21b942dae76ea352d
0x8d31550863b9bdf7a75ef81ce9a395e14376842f
0x96a9b72547480eb346d53c01acc781d8f2f0bf9c
0xee525a275d1f54c22cccf1a3314f13c712d7f3a8
0xceca708fefffc842de98454c3ac5dcfe342c3f67
0x7c1462c014d12ce8114c8d20897746e418d0609c
0xdd534250cc5705f8751917ec9e400d715ab6e171
0x2825861682f978d5df5044c42df6a7fa56f43933
0x4de4aaa78d97d2f471ef966abba3ee26a5233f71
0xfe3766d4b8f8bf029d4fe4d355be152f9c67eb90
0x97372ba157f00034cf4c38791d3d828a3194fc34
0x8a2ea925521c111dad7e328a32c238898589cf3a
0xd959eb5165d88158bf0643e6618fab4120fbd810
0x3afdd164605122f7ee98b9197b9761d26a8772d7
0xa891022919e40e9d6ff50dd027c07d9b37e97dcf
0x7591b5105aae76ff8e8a601c151e5f7e1df48ce8
0x4fbe804fe264802ee3332687f56abe755c265b94
0x13daea54537ccb33caf9131812d0441caa2ad63c
0x953f368f1013a40a8ade7b2e3b8d73e9c7e1f701
0xfa699091d82933d5ed9b980d7eb1fc2341d05875
0x12a8d9bf53b1685c262e8979aaeb81adc20baf5d

```
<img width="701" alt="Capture d’écran 2024-05-26 à 15 32 32" src="https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/63f45c82-e5ce-4b5d-9d2b-299e98606755">

<details>
<img width="1391" alt="Capture d’écran 2024-05-26 à 15 37 00" src="https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/296b64c1-a5d0-4de4-8c16-d45d04fe7a29">
<img width="1389" alt="Capture d’écran 2024-05-26 à 15 37 35" src="https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e5438659-e89a-4d79-8a12-6882999c65f6">
This one has a typical Sybil pattern
He carried out his first TX Layer Zero on the same day on several batches of addresses
The date of creation of the wallets also corresponds

21/12

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a1502862-5e83-44c5-9215-407e00489055)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/06778710-d763-4998-8025-83415f6ad688)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f67b8ada-18ed-469d-b522-109e60da679d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/89fb0cbe-1af3-44a1-b96c-51283bc08e59)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/cf3dd6b0-daff-4977-b3d0-7277e56523fd)


22/12
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/09de07fb-2efa-4fec-9cc9-07e886ec5365)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b83d29a5-574e-4864-817d-b226448a7deb)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0ab38d31-d2e6-4115-81b0-d66babaa8090)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/fc1db7a2-0c7d-424c-a407-6c8693e2a926)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4739ab60-14ad-4ed4-9ee7-be11ce92d9fe)



24/12
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/54d911cf-36b5-4d2e-bd1f-48fe077ac5b6)

23/12
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/37d0ed35-ab07-4f06-a34f-109c9d9cf2ff)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c21accb2-cc6a-4970-b8c4-29c1889583b4)


27/12
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c36cf181-bbb3-4bb0-926d-e36bab4545a6)

28/12
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/86ba5a0a-f7e8-4276-860e-516348ff8cc5)


29/12
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3baefe94-af92-4b87-a916-12e42698c8a6)
30/12
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/089fe85a-78b8-4708-a7a7-cb555a85d066)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0a2b9fdf-78fe-47b2-a716-d72e91a757fa)


</details>
Reminder: All these addresses share the same OKX deposit address

Each screen is a different address, he started farming between 12/21/21 and 12/29/21, he then continued his farming in May 2022, which I did not paste here because we understand quite quickly that it's a sybil.

# CLUSTER 13

The first 21 addresses within the cluster are linked to the same OKX deposit address: 0x151c6d618AF9305CCa87Dac37578dDC9AAbD9382. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0x5d30f88f92baa8a2bcd99e9ddb6e54e2ca8abb04
0x90d4aa3bf552999e7ca9ce89cf8e6fada4c69aab
0x22338f6036bd28d10e4180735fae96346283c886
0x2600544f150db80438004be4bbc7114aa21615a9
0xf72390c118188d6706bb303606c06457f198bf79
0x3ae8e01536785f47eaa87ff1542ee509671ec8df
0xeb3843caa198420fbbe5a023541a43bc9e8ec01c
0x7aa819e41693e9f435ec7da54e8cfd08d03dba6b
0x11a9ad3e94ce7a21f5bf14174e328bc7c5eeb6fa
0xcf30a573e3ac5e855fe23bf85ff78ef62db9e52b
0x3b5c6db44c2e63309e3c570b0f7c3569d2371ffa
0xde765b9d2a5b5b8e9e952da5ac3e43b011cdb289
0x4ca644b441749ac1b29a26f2189ad7c29435c20a
0x391ecebb351714ec949795f63d093b05a124c3a2
0x058b9c1ba7cded2150335464ca1951cf1ce38fde
0x0aacf7dd8fbd05aab11e3c6f170f9213b701baef
0xfcace87fb6e1dfeeda16533cd41ee2852a0f14b2
0x10bea37df7bd76a48ca5fef2f124fb177cc8683d
0x3fa4a5319fe925770965f5a4d12361cceb39311e
0x6762391958d87d5fa4d1252997615412a6a70651
0x0611133571496e814294cd17067f4c14eee7d04f
0x782f17e27322fb4d8a331f58f5d0e25dd0484a23

```

<img width="665" alt="Capture d’écran 2024-05-26 à 15 49 41" src="https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/21ae01c6-f1a8-41c9-b0c3-7d2e20f718ed">
This one made several small batches of addresses to farm with. Some share the same creation date as well as the first transaction date LZ.
<details>
<img width="1375" alt="Capture d’écran 2024-05-26 à 15 58 45" src="https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/344ccebc-e099-40b3-996a-a44187a3e76b">
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/be5eb714-d3b4-4cd0-be50-8b3262f23977)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/705fdf18-4ebd-4a35-b5d6-e2192e9ea5bb)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4de48bab-1a13-44f0-8b29-0f687034450c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3f7f8ac3-24ce-4407-bd1c-af568a9e467a)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/94aea1e4-6527-43bb-bc4f-d19a02eb9ec6)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a3d82126-5103-4cb4-a40f-abac7d3ffa4c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/fa4ef05a-3085-4270-bef9-e1302068bd93)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ee046199-efd8-4bcf-9e50-01fcfa2ccb7d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ac94ee42-4e29-4925-b593-d7738fbf92e4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/47210213-d155-4670-8823-d905f77965ff)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b9352cf4-4711-4958-b348-aabfd9213ee5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b60f4975-c79c-426f-9dc2-9474d7710d93)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/13fcb4dd-4791-4555-a340-270be34e7fab)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/dfd701ba-c365-4a55-8bcb-e73b7f1bbe97)

23/07
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/71f71deb-74bb-4602-9c3b-e12e92d3c78a)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6dba30bb-0b63-4a5d-b960-e75552397ea9)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f940915b-f44f-4bc9-a468-723a424e29c9)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f29552b7-cd35-40d8-95f6-306dcfe4bed6)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e8a80076-87bd-4a64-83f4-bc7f97874d30)

26/07
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4a6e67b3-ec1d-4655-8f6a-8860c64b5221)

</details>
Sybil cluster script farming multiple airdrop, across +20 wallets. Here was the proof with Linea bridge.

# CLUSTER 14
The first 21 addresses within the cluster are linked to the same OKX deposit address: 0xFE7135539984Bc905Dd82c4b69244C59c41aA139. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0x048489d28a0d34682002c81e0db50ddd4fec43b9
0x9810961e922035408301489c40b4fbad94c17221
0x6091a224ec0e8bae16125603d179d9fce7aad641
0x1110d50258fc6977857f6c12677c6e4e8303e413
0x86d0ae0ce5e53b0d9579235dc1347e574d73d2f1
0xa33bc5bf2d127b3083c4b76854fa8cf028c38105
0xc18f0ed65cf1b8c87dfa7f4bd66d7dc67ca79004
0x6350b602387f06c4c9ef1f983c80e8c95e84ce85
0x3d6f33e23711af618765d31ad762ded15ddf9627
0x4e3b67e8683b888f018d1655593640800b9eb067
0x1a6ba5a92de66529d33556c1704820449cdb9091
0xc26df7194f6b8077676643104412271e6e4daea7
0x3abd61e671bb0f195e30da85429069af02680296
0x5199767af87d0b974bc39495036d98ce82407f84
0x329cff62a0f725d00eb9353bae90722f1848996f
0x7ecc4cb42dbac18d1fd68bd6000f91ca93482acc
0xc6267fbd804b767d6aa0a6d294a150e53415c4d4
0xc65be4de0e9149a29835a51095283ced69ba0a3a
0x9ad26c4ec69e281ca74bd66a377fa62e7380fda2
```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ac472ee5-76e0-4a14-a699-0e57def0c6f3)

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/eb00dfce-90a4-428d-9929-4228c26ad3ae)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/aca03592-6c46-4e2a-9c4c-29bd5debee6b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5e64a303-eb31-49dd-a9b5-796b4629d9a5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3e2a9855-5b7b-4d14-948e-07306b4cee61)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ed4be1ab-f739-4b17-926b-9943471a3721)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3a4aed07-3153-496a-b45b-4243bddfd56f)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1880610f-36e6-4805-9070-30e988868468)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a35ac1c3-6a08-472a-a1a7-c74a171dd027)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/12233100-f5e9-440b-8887-7c9920c2e17d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e526f198-d7c1-4f4b-8ddc-ef7229aed28d)

</details>


Airdrop farmer caught.

# CLUSTER 15
The first 21 addresses within the cluster are linked to the same OKX deposit address: 0x1a7cb54e27dbBCBF5b3C24C91f36BA9d922f0b92. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.



```
0x8abe5c1b066b30069838e8ba35f2e4b02db15d64
0xff758cb857571ba5fe7891cdece84346c698ec26
0x875484c305e532a485ae6f79bab05e4677c15be5
0x9a9b64f79e9f2ff806da3e912f826941b39404c2
0x9a5350aaeb4f3a5d896783b4c122919a7d0f9f83
0xe205473109564210b726d5227ea56c92c4eb7ae7
0xaedb26f3d279529c7670f2761ffea889f4c1798b
0x834684ddb8c11eb58fddf1159e9c74953b892cfe
0xdcd993c9482fa22a873c85a7018044106e1d6fa2
0x6a21b81376ef4759f2635a8f6f3c9858cea457a8
0x8c6a9e2006bd71989967854cc5fc9dafdeadf64c
0x0cb470a536e6e48333f7182cc7fabc945a2cd93b
0x2f6c8ad9b90f03f1444f8512e30f48dd225f0dbd
0xa5bedade8c873b871d08f2d4b1684a9bd6945ba7
0x21a9e6f106f4d4247db9462ebf2c9c4241578da7
0x93da1d0d77e7483fb199cecd0b2077a58ab9abc1
0x8f55cd4e6d20db42dbd868865686027dd346b97c
0xf0579b201b2baecdd6472eb044d9b96f6d314779
0xacbd8887d3d14c90573453074e7098a909a3fa15
0xacbd8887d3d14c90573453074e7098a909a3fa15
0x1a7cb54e27dbbcbf5b3c24c91f36ba9d922f0b92
0xe56426b87637b5f516c9a4b6b1ce1b914ff197c7
0xdaf393b0082922d75465c2a08ba6f93f47c54918
0x09f31c0aee729ba208971f07bed903b0d0135e4f
0x326c1475bce07e9929797c35107baa3dabea709b
0x54cee5080bfd348e2601a36c146a5dcfa7d8b106
0x61fd3f38d60effd953b31e531fb80eeaa37a285c
0xf833c34a795c0b5612af027e23800e8090c64934
0x0c7f9dfe5f484dc75eedbb76d1fcdfc8970d0cb7
0xccbf77fa01ea919a599eb8d0a68d12a3e277a5d2
0x0fd32cfe822823b7c01ee22fff31d27c6f6b1a8f
0xb9fbebc86634184448742c918b127672071a6f19
```






<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f09b7021-9006-4ec4-85c0-f4cd1513c689)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/10fd1483-d672-4e78-9fce-337ee33698c1)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e0653387-7ce7-4569-8df0-4fcc8d7a9913)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d3817ab8-3995-40e3-a2db-8042ece44130)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3f3c22ca-edf9-47d9-9a02-915f5c2c3988)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c27b38f7-d87d-4f43-b65d-620897ac754c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/773ec8f6-f3ca-4c6f-835d-4e75715b7297)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e9041c09-69a1-433d-8423-9c86c3fdf5e6)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3692d0d9-ea90-428a-a859-1668af0cde2d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/14a0eeeb-0947-49a8-9c4e-5a165e9ee583)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f593ab1e-deae-4ae8-aedb-2a52dda20aa0)

</details>

# CLUSTER 16
The first 2 addresses within the cluster are linked to the same GATEio deposit address: 0x3949fc515d9458a48a64d7a0338f0ae65811e759. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.
```
0x63c24f164fa69f4db7f45f211a8e089c157b4747
0x600d1bf9ad00514196ed9a96c5afbddb471478c9
0xc60b220f62578df2e584349dfb3a771780a300ed
0x8d1d836f06d271028d028b4fb7ba4386795b9d0d
0xa872e46e6da69402303522bcdf9f4538d16175ed
0x4e91394b30162d5a63a09f5cfe253a09d05254c5
0xbcc543e49afbaecfb65f4cdbeac271a97e735f45
0x6216977058c2a6ce9b910a119f3d0131b0e7889d
0x45f93ad7124ddd2d578e40de6f0836548433707c
0x3d8b8ea64af099a0d2dfd9f0c97164628ee422e7
0x53157a5ff07955f323a7624ae81c1add7e15d9fc
0x6e2ce22c13eff481456db5c975fdd0e3f161f611
0x695aa322e8b30aef3a0a417bd49612fc69b9313f
0x427da433d001c8e4e4991a544575dafaf493399d
0x64ea7be4d6ed0621aefe1ffe6d7d38e9a6396eb7
0xc9f308d054b9c66a65dbcc1878772707ba96135e
0x327a8065328da20491ff01a7735733c8c39bb685
0xca8ba91243bee135fdf59fc509b27fded695c387
0x2c3d78b8ab518d5ff6b909343f6865df41b3dcf0
0xc1e66188827800152f5e98190f9c59c9ecbcfed0
0xa4bd43301b38698faac1a179f2d2729e2ebb2dfd
0xcdac5fa9d6f811a1e63714b0d4fe7bbebe07df0b
```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c2fb2b42-96c7-4b61-a301-48ab23d309bc)

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2e4fc35f-b063-497c-8dd4-edb26f3fe946)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8fc03e5b-6d75-4cd9-af68-2ecda04da1e4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2492ea0b-1306-4bd0-911f-ad18d19152e4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/af4fafce-db4c-48de-8980-52b22b49e1fd)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b0bbcd65-ae55-437b-b9f9-a49c72455db4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5874d6d8-5469-4158-8122-25de37d8f139)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c335fb89-3868-4e91-9305-8901c8f6afdf)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ab0bbdad-41a8-45d6-8dd5-e47b5114894d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e758a39b-53fe-4f7b-9dff-e0de3f0ede18)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d1c1b3d8-66ee-4061-9961-3923e98f9827)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/37d3e3aa-4010-472f-b708-8dc8e70f7686)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a84581e3-24c6-419d-861d-67da77de4bc6)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/83fe5143-2540-46d1-931f-46eaa53192ab)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1ee1df9f-6698-4b47-8093-c14b0bd231f6)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e89516fd-ee34-4969-867a-59de7e3fc0a6)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/194e0d9d-6626-4b55-90bc-8f4e90e7fb4d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5d5c5132-f70c-4870-a562-58cb8f588aa5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4f219b90-cfd8-496c-b3b7-4fb6131e7891)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/562cd390-8b2e-40d6-9867-e3491db706c7)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/26af7f1c-8c99-4298-9816-741b55bfa12b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/27fc5cd2-6b04-44c7-bd91-89eaaa62148b)

</details>

From a withdrawal from Gate.io to its Gate.io deposit address, via its 21 farming wallets. The perfect Sybil.

# CLUSTER 17
The first 20 addresses within the cluster are linked to the same GATEio deposit address: 0x936aa3d5a6658F6Df4FDDCa9Cd6BFb457D8b23C0. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.
```
0x63c24f164fa69f4db7f45f211a8e089c157b4747
0x600d1bf9ad00514196ed9a96c5afbddb471478c9
0xc60b220f62578df2e584349dfb3a771780a300ed
0x8d1d836f06d271028d028b4fb7ba4386795b9d0d
0xa872e46e6da69402303522bcdf9f4538d16175ed
0x4e91394b30162d5a63a09f5cfe253a09d05254c5
0xbcc543e49afbaecfb65f4cdbeac271a97e735f45
0x6216977058c2a6ce9b910a119f3d0131b0e7889d
0x45f93ad7124ddd2d578e40de6f0836548433707c
0x3d8b8ea64af099a0d2dfd9f0c97164628ee422e7
0x53157a5ff07955f323a7624ae81c1add7e15d9fc
0x6e2ce22c13eff481456db5c975fdd0e3f161f611
0x695aa322e8b30aef3a0a417bd49612fc69b9313f
0x427da433d001c8e4e4991a544575dafaf493399d
0x64ea7be4d6ed0621aefe1ffe6d7d38e9a6396eb7
0xc9f308d054b9c66a65dbcc1878772707ba96135e
0x327a8065328da20491ff01a7735733c8c39bb685
0xca8ba91243bee135fdf59fc509b27fded695c387
0x2c3d78b8ab518d5ff6b909343f6865df41b3dcf0
0xc1e66188827800152f5e98190f9c59c9ecbcfed0
0xa4bd43301b38698faac1a179f2d2729e2ebb2dfd
0xcdac5fa9d6f811a1e63714b0d4fe7bbebe07df0b
```


![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/39ebce12-4550-477f-b6d2-6f9b6d36f8f5)


<details>

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/73fcd1bc-cd42-48b5-ac03-ea6134de94d5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/41be34a7-7e47-43f2-aef7-b4324db0fdae)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/866dffce-8735-43e7-8aea-2d0ab2335766)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/7de39fa0-7b0d-408b-bdd9-5129a8bfe30a)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/20124082-89d0-44c5-b45b-656d387e10a8)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2552ceaa-7e46-4749-b3f4-42830aaedda4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/47b21083-43f3-4260-9413-42e50413fc8e)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4e7af542-2533-4474-8699-c36beb4d6f7e)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/07890a22-e36c-4d6c-8d69-e370b949b3c9)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0e5b6903-b133-4b6d-9e82-b1c5f6c0036b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d641f8a7-f12a-4a6a-87b0-1be5a1c9fb2d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d910677b-3a92-4625-aa6e-b96e0c5fc79a)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/38a79a25-2d07-4fde-99e7-8961076fcc14)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c3c62a24-0c54-40cf-8bc9-927e7b997e1d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6fcbe7e0-5a36-48e9-8f71-fa480250ef49)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c8e1404f-6fd3-4e9f-9527-fcac5652613b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/90244b32-52c8-49cd-93f4-73ae48122869)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b16a6457-275d-4a9d-9abd-09b72a430a68)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/40aab92d-ec8f-40a2-a82f-8d02be132b1c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4b84ecf9-d590-484f-ac66-ad4ae876adb8)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e0a85d0d-10fc-418f-9274-d59dd23438cf)

</details>
Cluster which has the same pattern on all wallets: Activity at the end of February and the end of March 2023
Deposit then withdraw on ZkSync lyte

# CLUSTER 18
The first 20 addresses within the cluster are linked to the same Binance deposit address: 0x948Dc867B61a2317752cF2F7B6BEf0C708283555. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0xe86c0fb64477b16a7c4e66352d8f2d1ac497b72b
0xe04b83aa59778aa331612b79f6f634066b4b427c
0xb70a7168ac7720127524e3350e0e128085ad634e
0x0a0bd78196d3c423e05e5acdc94be0a5d71cbdaf
0x502d21270b59659e793ee579ed8f37ca88888a21
0xd1632f3716a26c78fdaa074ceb0d4cdf4bfdcead
0xd488e548dad8e1b0845cb1b5b71171acd74ffcf3
0x21155c018e4eb0efc541cd607b5ef5a176c4d70b
0xf3db711f1af8dd2aa554ca2764a36c1982d65ac4
0xd7656247336d38c78d6356c9e98bd001c8162a44
0x0125e36e0515a84b7a4cacb463829b8dd41bd314
0x461ffcd712c8f566ea88a4c41de69b5664bbc2e9
0x29a5406b7bc30576c24e91cd45b3cd1679110fbd
0x4bb3d966910f5171eee89aea00b7e46664427f5e
0xcf1787e5718462438eaf880cb63f03be3040dcd4
0x670ed8d1f94591217264951721b789e0c4cba7a1
0xfe2623b65c3433f4a1ea810e29bc6cb040a9c94a
0x1f8890996214d439b3d9e3c6704485625b21738b
0x43e2383c0914ec47600fed79d4c3534b1b646eac
0x5c08e14f5741ff7ceea43de66c3c5008b1355e9b
```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/376fb085-5dce-4f92-89e5-edf9ec4a4d04)

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9577c955-7e80-4028-b905-1130dadabbb0)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a82297bb-d9d6-4be3-abb6-7fa6724f059c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/207ce2fa-689a-41d3-974c-5f29fd015ecb)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/07f6bdbb-7592-4629-9e67-889ba8b5f263)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/801d80ff-7bd0-409c-9ea0-10aa7ae8aa80)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ecb4a968-2dd1-4800-8e0d-25089092a6d6)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/24a6422c-62fd-4c14-8b29-8371cdeee7a3)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f891c03f-f93b-4de6-a9bf-91f60fffa51b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/bc393e8f-9f8c-429e-ab2f-74535f937349)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c28677d1-8972-47a5-8f09-37f1a258e500)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d80a1530-5af0-415d-b39d-d9f39f974398)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b9cec354-5a72-48b5-9927-d0261d995541)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8d5d5cb5-5bc8-415b-97b2-d7493fb95fa4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/864448f5-6ceb-4472-bba0-e334b5d39589)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2e84556f-0749-494e-8f06-f22c431d1125)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b0ce382e-85a8-4f5d-91b5-1c401728be9f)
</details>

Sybil who farms different airdrops, same tx with the same amount on the same day.

# CLUSTER 19
The first 20 addresses within the cluster are linked to the same OKX deposit address: 0xB07CE99131AB84b3a60C53Bd8c462c0E4330cACd. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0xf0322775dc5a0019d88ba301578770c637ebbbdb
0x3d3311db38e3e808075e19f48bf3d2dd487edf44
0x767362a9534fafc17d9e0c3e80356be27d165d94
0x868b45fd96aad238dcde2973a532f2539a7a8834
0xf9a1a1ff90d66bd15b8bfbde69ec8c052fc3301c
0x9d2034ff087cd64f8b3fdab078dbccd2e2e466ae
0xc62039fd8b0d5ef1a68f684e7cf6c13d7ea6e8e3
0x1ff0d508ba846575e738039b38f778c23e9ff96f
0x163bc8197e0120346b07d22e98bf552946976d69
0x3cf29fad5588785c55fab71d802a07947095264c
0x9ac5ccf1e64a7709849130f10074a5772c90e421
0x297554a3e38c48450e72ac043dbe8c2b602d0fb8
0x9252a2772d8c4fd04081afe76db8f1bc0e6ead59
0x4a16fc8d9ea4837400c27b82f5a4fb3e4cb2c117
0xf42060f1ee25b56d3c99a9a3bf7c6e26c64b4ed4
0x94e53362650fefa716a5ec07b148ea15472e19ba
0x8f7d339bbf51ed4a57549c71aa5648dbc56c3efd
0x8a519e59fee768982db71a79e074f1ead90b9e47
0x125b4e10334088d27ce554de13ef56a928e0747a
0xec0d8d0528419c7fb77d8e6a5bf55612a92bc84b
```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/7a655bcc-ebb2-4302-bca9-9826cdd36fca)

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4f6d691f-2299-4408-b797-0eebfa8745a3)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/80a52318-10c6-4fe4-b819-f749998dfce5) 
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2972d601-bd54-444e-b447-a19528bb1d39)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5b5d18ac-180d-43a5-890a-157f969315e6)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/53928e4c-e104-45f3-bf84-eadfbeb8ff22)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9630879c-2ede-470c-a3ec-417f735633c4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/06739441-4ef1-48b3-a71f-e6411ebca84f)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1fa412e0-f708-474d-bd47-be7a5cb487f2)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2c4fdfb8-4662-40bb-882b-8160af27f382)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d42cb246-e50f-4d1a-8321-1acafc0882fc)

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9370aa99-5131-4b6c-a0ba-c6eaaad806d4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0cebb1f8-56f2-493c-8d0e-83da1eb01709)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0a98543c-8754-4731-a1d8-5a56d41996e7)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/efdc283d-ff9a-4cf5-8273-ff322e793bdb)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5270fc21-e8df-49d7-a0d9-beaf2b7e3835)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1cbf578a-a8c7-4edd-aa4b-40825d790198)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/01614d07-d818-4fdb-a567-fbac70bae8b9)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/64ea6204-8c06-47de-8857-8d536270a8e5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2e31a7d6-965b-437f-8aff-e4e527be3a9a)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/37b3f69f-d137-4173-8da3-cf5391f053a1)

</details>

# CLUSTER 20

The first 20 addresses within the cluster are linked to the same OKX deposit address: 0xC384C95aE4F03a686D6f547aC8569D17E7bD60Bd. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0x6ea297b1809b54b7d53083ec07f4a6a2b54a71fc
0xb93f6e605b2a5d55fa83b2eaf6ef403730d633d9
0x7dce8679e030b5cf4d5df615afcd0b084a4b16aa
0xea1ef14d2dc7db19e11a2515c4bec40dd1c37e20
0xdf2a22d616ec7013ce35fc79b3ae27d8a431339c
0xe007f05f1a5e333b5b20de19f5a45c945e642b33
0x18f5b949f6c6dafcbb0e8f43a1518fa5fc39bbe4
0x6bd206f8af3f80c32522a49b0fdf9b1e10ffa1ef
0x36420e4f8735fd65b039d5fea7f16c401057aec0
0x84641d5fc37c6f85057461020e3cfeb1c35a3d41
0x1675c0d30dc5dad8e38d95ff189f85314084d6b3
0x5d6c92eccf40953bfb9d81d0e8c31e6770a1b771
0xc395b4e55deeabdb22a40b554c3b0c0fda7e7e63
0xd4a077bc564e49562d8d74391451a0b639dda404
0xd5cbc980eab7b79f7abb849212d7e3b1a105e5a2
0xfbd059e151fac920e53d6a35f4d51d5b9477bbb9
0x1115855b863452525229c57b58dc95690c893690
0x90ddd3049725d1d8067e4ab5e5eaba7773e58f9a
0x619bf38292c0ea870d8e4815ab96a9ffac3b2e19
0x6622dc3d88683fc475d09d712b2bc6b2027ba47c
```

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/db2cfd5f-a393-4291-a776-4ae95d265bb2)

<details>

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c9d4473a-2bc2-425d-a082-7c9a701f1e70)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/20626f7f-e08f-452f-abe3-0147a4c14b3a)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4cd975d7-7841-4a57-9c1b-4cf9f4a577df)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/db76a144-f7d0-40f3-b58c-e16412a87e59)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6418423c-6a27-4720-824d-2e8fa0e7e9cd)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/03aa4fa7-d69b-4f3c-8a35-94d185aece3f)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6c78cb13-501e-4a39-ba26-e5e249fe06f0)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5ebce045-8c87-495e-a232-82135314b27c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0a01f872-fb2a-4e65-a756-ecc948c22fb7)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/afdaeea2-71d8-4fbb-932f-6a2be3881bcc)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d3d1cd0a-a376-458f-b150-870de9b3cf8b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/95e22cf2-a293-445a-ae60-149c8e085708)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1c14584e-a50f-4044-82d9-a340a32a7ab4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/053272b7-1725-4653-93fa-9cae653e6a81)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e1b3977a-eaba-4474-b998-7478b9b1b419)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c8d77c43-af6c-4997-947d-71186640dafd)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2e93da66-f14d-43af-ac6a-7e7dd276fa9d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3656223e-4a1c-4cae-be01-43d134ccea40)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0737b07e-508e-4eac-a0f7-4d9060173930)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/7b0f62de-6d10-4ced-bf85-ade439cc643f)


</details>
Sybil detected thanks to the Zksync Bridge, he made the same transactions on the same day.

# CLUSTER 21
The first 20 addresses within the cluster are linked to the same Binance deposit address: 0xBbc0461EB0e3a310774bA46756cD11E348A27F26. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.
```
0x0889ffd6c0c90adc3659cb9efd8b76f7d0bb20e9
0x8790095322c6faf74e3fc983506f62f628fb0062
0x0826ad353b9c6b005ed697ae9c9e06c2f5798c38
0x87fca40b60955f304c8429c5757d8180dd811582
0xd6401cc0ca7eab0efa76135a7cb5959cea5bdc2e
0x90296759b03f32d3783e93eba20db8b9a0c26b49
0x6c43433a490ed270f2023143be8a8c2f61f66e57
0x9840d7cf3a261bec056aaaf0e587cb9bd4ec5b3a
0x1ffff42907fbe7d500d113e864b0d299255516bc
0x9796c8bb6fa6200e420e8bacc2eaf7c1b26e10ba
0x1551c6b351f623ff6c8ac88f4f4d27d03f0bf8c0
0xe587005dfa23af2fb98a3de6aaca66037cdd8ebe
0xa63757ad9c3078ae8d34b9101f5d7de9fee96ffa
0x94f88de76529b79ecdf15d7ce9c783f8b82cf282
0xfec0e78062f14629f95d1abbf7395bb9de3f2214
0x68b7cd166fd11e7b84fd8cc80a16d51e6b341e27
0xa029f864170011e9d761622d97310957b56889ce
0xc3e1696990e7726375f5e0ee886a91bbabfd32ac
0x0d541f8226f066d723afad32e4d540c2b3dc222c
0xdd6536a6314578a2ebfb1fd6f166a65d38351ce0
0x7ff4c55853ead02e504b5bb48040de5100c616ad
```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8ce8cd0d-a4b2-4306-9eb3-1b174434e7bd)

<details> 

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d0629a46-e858-4be6-bcd7-46bae02c1f8e)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f3d0dd4e-dd4a-424a-a76d-f79988c83944)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/bda9a951-311b-4737-89a7-d87f30f107fb)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/51c26598-ca07-4d4a-a8cb-6da218bafffe)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b68e4388-9378-4a69-aa1d-b420e7b4bad8)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3a322cb6-ef5d-45c5-9b83-d29b2fd4d459)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a7ad30a9-d514-45b3-9922-62ea58d9d415)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9f5e0816-6f8e-45d0-916f-297bfc60c138)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0ac5a05a-0680-4991-a39f-d36ec1e9005c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/7a253c3d-1cb8-429c-ab74-75d1e56d5a74)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f89a999f-974a-4acc-b54a-f5700bc475f5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1e0cdf9c-c21b-4667-a36f-e4d19c37350c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/823d4e1f-2c5e-41ce-8afe-44206e42977b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/201580e6-019e-4e6c-b5f0-e4168c1335b5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5423996b-10ba-4b75-9c59-312f7e19179c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a80f2459-32fa-4c16-96f2-483c82fd0697)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1e846958-a429-453f-89de-87f3ca64dc80)


</details>
Same pattern of create lock then add liquidity on Stargate on Arbitrum, Sybil 100%

# CLUSTER 22
The first 20 addresses within the cluster are linked to the same OKX deposit address: 0xC384C95aE4F03a686D6f547aC8569D17E7bD60Bd. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.
```

0xb93f6e605b2a5d55fa83b2eaf6ef403730d633d9
0x7dce8679e030b5cf4d5df615afcd0b084a4b16aa
0xea1ef14d2dc7db19e11a2515c4bec40dd1c37e20
0xdf2a22d616ec7013ce35fc79b3ae27d8a431339c
0xe007f05f1a5e333b5b20de19f5a45c945e642b33
0x18f5b949f6c6dafcbb0e8f43a1518fa5fc39bbe4
0x6bd206f8af3f80c32522a49b0fdf9b1e10ffa1ef
0x36420e4f8735fd65b039d5fea7f16c401057aec0
0x84641d5fc37c6f85057461020e3cfeb1c35a3d41
0x1675c0d30dc5dad8e38d95ff189f85314084d6b3
0x5d6c92eccf40953bfb9d81d0e8c31e6770a1b771
0xc395b4e55deeabdb22a40b554c3b0c0fda7e7e63
0xd4a077bc564e49562d8d74391451a0b639dda404
0x6ea297b1809b54b7d53083ec07f4a6a2b54a71fc
0xd5cbc980eab7b79f7abb849212d7e3b1a105e5a2
0xfbd059e151fac920e53d6a35f4d51d5b9477bbb9
0x1115855b863452525229c57b58dc95690c893690
0x90ddd3049725d1d8067e4ab5e5eaba7773e58f9a
0x619bf38292c0ea870d8e4815ab96a9ffac3b2e19
0x6622dc3d88683fc475d09d712b2bc6b2027ba47c

```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/be287f25-ccff-4c6a-8920-33be575bbcf8)


<details>

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f4e1e45f-7e9f-48a4-8b55-54552307a4c5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0b5e6197-d598-41cd-8780-1c8dda4c93b3)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f0702eb0-42bb-4d9d-bad0-20cf50a3d532)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8d6be816-be4b-4353-9817-acefacab822e)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/54984272-069f-4b37-a6aa-4aa12ee1fa84)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/546e0be7-abde-43f0-870b-8062486eb3ab)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/33f097b1-fbcb-4513-b13e-bf12d96e5e05)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/39f7a57c-7c9f-4c8b-a8a4-622ad9c4317f)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4c7363db-13e7-4ae4-ba40-b3508f1dcb40)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ce1d4022-0ccd-4db2-81d9-fe16cd49484e)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/135f2670-6b12-4376-8f0a-36fbc11f68a4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2894e2a0-f8e8-4ff5-8985-bd6041a561d2)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6a1be35b-18ad-4dba-a12b-b1471bec4112)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/59be895b-16d4-44a7-8f6d-50c3fd4ed7fe)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0c21219b-7858-4d13-bdcc-7de91ea5a8c3)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ca53c292-ebed-4659-b255-43bc4aa8fa61)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/7007bd59-6c13-4770-9b5d-27190124b2a3)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f5b1bef3-6033-41c7-80cd-6b33e7f60582)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3a38d5ef-3682-4842-a7aa-98548106ca8c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6749b748-5e74-43b7-b4fa-17ee410ad1be)

</details>

Same pattern each time: Uses the Zksync bridge on Ethereum on April 7 2023 then Bridge Back in January 2024

# CLUSTER 23

The first 20 addresses within the cluster are linked to the same OKX deposit address: 0xC462149B86266346845D04243455a7dD9Cb35230. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.
```
0xab3f80328770a2f2cf8148f7ce28a84834ff66c1
0x5bc63079e6661145ce2ec4807d2644fdbb0a0c27
0xf8082b76dfefa3e4e649974413ddd00a8dc408d0
0xb347e46b391301657fe4f3ac722b132c009db76f
0x99e7d1319a11374fc0a64f46f4c7b1edfdc6685c
0xdca4f50095015219e4380cbeed9e2ff4611b6bb0
0xd4b9ead8f62f3d2db27a10a9b9e825118c6c257c
0x84332bb78ca5740f45c4639f3066a0d4529328bb
0x5fe20406c7a4423109314fb17d2708b0bee8535d
0xac6277f5a9dbe3e81d27146cbc2aab2b05b76a6f
0xa7d9ba18f3e7e901e987265256ff1b0cffb043d6
0x03d4e412d3d97963aaef18027870e33f51521040
0xc043e96110652b1cf0d16c7f69724e869f6880e1
0xba3f923cd7d23dadf55830a74eff100306623152
0x4db34e3cc4b77bc52bc8c9f8d79f6fdbeb53c47f
0xb2a52b874e88ace933640429e537e216c99b382f
0xef507e6334f3b546aa47b926cbc7fce5c91f1c6a
0x8bcc1bd467272de53df513eedb04aca0fe272a37
0xf11d53f79274e801a14c2a7a664a2a555c663bdb
0x952ddc9ff6fd62ada843146b8b3333e841a18154
```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8fbc6174-70e8-492a-b0d6-fca7d8f00ca9)

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b13fe6fb-49bf-491c-a092-916e74bfd61b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4401efbb-8de0-4802-9afe-c97778e35b2d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3ae8f402-d22d-4b6d-87f3-852a918206bf)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6d1f1f3c-d214-4294-a79c-df7c9d715758)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/42438563-2683-4dfb-a725-d9fe8eb2f209)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/bc123feb-371d-4d6c-aad7-4e529132212e)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b2186b79-de83-4e55-a257-c7bbedc18f0c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/eacd51cf-2881-4779-bd78-d3c01ec4263f)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2688f69c-b3ff-41b8-943f-6083a92363c3)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/7f1df24d-247a-4a69-8616-b8dbeb8ba9e9)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5f36567f-e8a5-4d8f-94ca-ed0f5bdd0f3d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d5bb6bc3-e9f7-44dc-beb7-1c78d0d883e0)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d98025dd-1be1-41eb-a1c4-e53f37ea6bf6)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/83d5b10e-b074-4c4b-a0b7-2dc047de8667)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1c2a4a91-5f9a-499e-a8f5-54580ecc2367)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/51be2880-80e5-463b-b3c8-e3fa6f71fce5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/49845eb6-316d-4e04-9d7e-58410c0fa546)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6af0c453-9600-4940-a757-581f69853adc)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/63bd8ea3-4823-4000-8dc0-a2be119fd204)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/14c04c0c-1832-45b4-8502-6417502f4339)
</details>
Classic Sybil who interacted on the same day, the same time on all her addresses with Zksync

# CLUSTER 23

The first 20 addresses within the cluster are linked to the same OKX deposit address: 0x33e100753f7be242b030db38d1432b2089ec2d0b. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0x33e100753f7be242b030db38d1432b2089ec2d0b
0xc75fdec78cfc441b549fbfab7a86a0744165adc3
0x2072922c71565097fe6848f9510192ea1c5e29b0
0xd7430f64b89dd4a8cea430b8bb56258359c146a8
0xda0a22e3e741d6c7ad8d6fe4a4889f4d9e8f79d1
0xef17afbeab4df151d9814aa45fd147b8f91e0b01
0x7d1d31fe23c5ad1c6a371f783d172b5383aaaa21
0x006798ec0eed617e69b8ef32c24221a54c4bb102
0x371f02a17b27877d1634f3b247e0c9809aba3c45
0x0707ca8af1e2b928dbcd7d40d198526b8ff8c6a6
0xee6753a91d68e7715f5e0da51859eb2655d37f52
0x09bc40a29969161134b5b97297f2ea6eb792d2f7
0xdcd7e55b15a4cf5be3e2c02e5ed3342092b0a976
0xa83e71953765f38b9e1fd1b42e3b181ccf69b326
0xb2a9e06e1dde4dad29423a74c0f0d82a8a336233
0x4902171ab55a5c1974422b0404828c3beefe21f7
0x0d70d61f4197827e60b52c3ff5f134aa26ae66e1
0x4ebcaf25dc546e3ef407df89944c1c91cc6bf6f4
0x0c317a092dbb21d1654c7dcf873675ef753c4b06
0xee92206c3d4072ac9db80cd45bd1bc302cd53ce7
```

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9be53530-abc6-4406-8b0a-12f55585f3ea)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9c2a9e39-1917-460c-a21b-1278f7dd9a86)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/5b3516e6-4d1e-4348-a1c2-3bfea84412e4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/1e43d901-db0c-4513-86b0-ed2776a145f4)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/22508bde-d265-4ce4-86b9-5bfa9bbd0f63)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/96303495-6360-4fde-9def-48fc35dbe47c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/aa707d6f-410b-4c4d-85ae-82f00582fd70)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0557b50e-d4e1-4152-8f4c-aebd9e1faf52)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0d292940-74f2-48c0-a417-99ab4dd70adc)

</details>
Same withdrawal from Bybit then bridge on Starknet, same day, same amount, same hours.

# CLUSTER 24

The first 20 addresses within the cluster are linked to the same Binance deposit address: 0xd5EA560724CFA15f5c9A5a9e851C08fbc98aE808. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0x5cf8067eae342ce64f5dafc659de21c1aa6dd8bc
0x86ca33cc0a554d870ed34d9aef7f2dcd402e3e7f
0xddd10e373cfa376eb3724698e08b8e4f302a0aaf
0xca2912ece1a57a6d33582a6896124b3b968c7f40
0x474380df0f203b7b7fe1b9d99c3821478222424d
0x9f1c6b7a6cab13f329498217d45fb0fa73d9c74c
0x531b3ca4af68d7be6e5b5c6ec847a037c1640555
0xda8d0cdbc30a8cf6274a3abbf1f618c1cb3a13c5
0xbee4ffbd5541c8937d883ddd89e6dd25862bebd9
0x6b97ecffce9ef660e140a2063aabb713af20991e
0xfd1cb7c8db8e2e216778edf45251be424ad8e694
0x3eaf5e1269e6e9497f200cd9e27ed100d584d507
0x31ebac9a66fe04946c18a9a8e0cb799e04440c27
0x1a37fdd0dbab21c5b6f7ec24f62e034d10100b0d
0xd86ec956f5960be98139569e1fc4f794bf973ac9
0xbed051ac1d39ead23cfa128563718cedc8aeadff
0x46d32c54f8ccab8f4b4e6d1e40da26ccf1e122af
0xfe027981205b09b40aa3aef5b4ae8c022e8dd2a8
0xae0a874dd8d47046602605311517ea287e1830b7
0x200a0f83302e08204397784b86c2de78267e2071
0x2e3c8ce5c12260b099c145cd8babf1441708bbdb
0x9d56315e5216963703f1e4b4169fb069ef701e41
0x1c0467d2f7fd720ef7705b69a43b97da0ee1e528
0x21cdb52f9258ea2ea74c4369a1e0c1dbcfd59e4d

```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/249f9ae3-3c59-4ecd-aed3-c7462c2a5782)


<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/569d1380-2503-4bad-a472-e0ccdaf351db)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8568dc7c-22e3-4e02-89de-5ae062a07256)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f4ac5886-02e7-45cc-b538-38f68fbb6ee8)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/48f86907-0802-4bf5-b48f-4cc02fa7b3c6)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/271d4fda-ab13-41b7-b7f2-e6fa20e0482f)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d364a942-a90d-4baf-9d22-39c444114e9d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/228221d5-49d6-41dc-9d8e-e2a057c12f35)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/fa1cd8ab-fbca-42ef-8d3d-8e8e30b0b4fb)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/bf0a8c0b-cfdc-4fb5-85c7-7d1a006202d0)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/0c3da7d3-7519-4aba-90b2-f163699d7e63)

</details>
Sybil which has the same TX on base with all wallets, one less

# CLUSTER 25
The first 20 addresses within the cluster are linked to the same Binance deposit address: 0x3D122Ee2D9F16C912dc293D0096841E96BbC5D6d . The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0x958e46926e797fa5bc01f9d3f23a0f34ee937492
0x4c228d587d60ff7c1b03069ea7ddda92c5c683de
0xda896291b98f5bc5195c61dceb516e4c18090a5d
0x3bdbde53ae1529fd865c451705b31a52066b6995
0xe6fe54de650af4762a176faa30b0bc79f1e8c385
0xe7bdd488fba50e76fdbc85ed33bbd0f0619ca553
0xb80fa36204da2149136875a626f82ec856fa2f0b
0x85229b28cb3308f952ecdb196921c93aea2c038e
0x9a0f37c846720822a5504bc1ffa722d385f8d852
0x579454d259bde515b125a5714f7fbc5e4adb1517
0xae74a3d99850ece0332bc0004e4bde52d87b35b4
0x2c93436ca5299bc8cdfa379004583a1bbd0e8e95
0xd079ebf3703f3741c8df349674b2e0dc8995a342
0xadaae038c946b83f8bebb06dc23911fdbb9af9df
0x448edebe5bee41895c723286949058c51076f9aa
0x4273cb9ec8153b71e6217c852ccabc2a93025789
0x084fca2aa53a7f2d2f260cf9422ab1a84d0cf40e
0x15a0418726b24c0b51ccb975cdd2f321b44510c1
0x1f9e87b17569bdc6a1e5c6f3aa6f3b1c4136aed5
0xba79781a5bb179809d741eece7006b79dd60dbce
0x35d970b0aebea71b20d66724f75b5726a7329897
0xa7b45165d2c2b71541c0299498aa5839deac2c1f
0x2967ca56d43957963f88da98850be610800163ac
0x21ff7e06f2b3549288c7eb4d418470b4cb7eb7fd
0xcecd7c994d4839345d4d153249b6d28b23c23574
0x86382f9bdafc01d58bc5faa3edaf4ea17b4e3a4b
0x2b1d16427a0f88bdb3f856291fce5448f7fc82f7
0xdbf4ecbd54d9b2b1e75492793a1122a4c5897609
0xafc17519b628dc17447f78f865bc21a43b783a9e
0x9fb115014d281f5afb5bc50dc8779c3480a0bd21
0x77f7b6d7f8f64cb67c9db02ced99fc1c930d9f19
0x07128d5d208c26d592195453c241783430f33334
0x86e083b4585fa0516933e5a4bcb500b61bc2691a
0x4f72e365218ed25b28ec5877098013b35e359eda
0xc47d1b221f7ad5686c1720263a56a67372e4b2af
```

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/8c6030c2-11b0-43b8-b8fb-d62c0764143b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9a6e0754-4aac-4dcc-a816-9b551a0c6f0e)
Lot of equal LZD 
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/26a0eba4-43cb-4c33-af2a-b6bfa1d17eff)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2768e0aa-029d-4550-b4d2-faefb0e3e46b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b2c67d7c-947d-4816-bdd4-806d4ed58867)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f5df6427-bd66-4f06-a65e-7b7c1a1e97f7)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a6d60290-3487-419b-a3ac-a8359fedd69c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ae28f7fe-662a-486e-9ddf-452972a14df9)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/44b4ad55-4fdc-44cf-a3e2-0e845c095297)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/bbcd26a7-7b44-4a8a-bf7f-7ce55cb5089a)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c4b1865c-3178-4a1a-8b00-831ba4f220d6)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f65686c8-1691-44b7-bde6-af2949da4bb9)
</details>

# CLUSTER 26
The first 20 addresses within the cluster are linked to the same Binance deposit address: 0x3cE95024Ef690e071a30e8745B28E80B2cCb6799. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0x5745eb3b2c96d72852c2efe336ab9b3edb7764ad
0x8bcc1bd467272de53df513eedb04aca0fe272a37
0x48cb93e3105fd104165d4ae145f84920391e33a9
0x818cf2cf79d65c0a21bb9b15a020009ac83f3cc9
0xf8082b76dfefa3e4e649974413ddd00a8dc408d0
0xac6277f5a9dbe3e81d27146cbc2aab2b05b76a6f
0xdca4f50095015219e4380cbeed9e2ff4611b6bb0
0x39a9d498743553685cde94f6cb01f6eb0eae68af
0xba3f923cd7d23dadf55830a74eff100306623152
0xb76f2104812fc81dc3efedf54053ecd783e4df1a
0xa612666e9798ec52eadfcee5fa9c85292fdcbdfa
0xa36aeebb132cdc486f0eb2627e8eb50e81903215
0x7dc66972b4da3296e257f03b004f03c615a50f74
0x1da87df3163755361db197c7ebde89d4c577cafb
0x34966603b65b838c1d8b284598bb281c37be43f0
0x934ec30a8eb232172166ea3f351e6291eec8b7d1
0x3d59a0edcd50ce436b6beab4f7d63c10227b7f23
0x43e446100d3189630711581fd521be36a9768ab4
0x93d5a2ad80687f84073cca63e71b4aca59e15f6e
0xe064f3ee060abb3b74c7e286f292d45043653b03
0x08d2f666538dfde37714ae226cf4e86dde9238d9
0x61e3a40c5fc49362c6bd1d8277b53728cc8afef8
0xb347e46b391301657fe4f3ac722b132c009db76f
0xd4b9ead8f62f3d2db27a10a9b9e825118c6c257c
0x0f8fc7f6a2c7e2ed44d72fe1afc65f7742f9d0cc
0x84332bb78ca5740f45c4639f3066a0d4529328bb
0xb4aef56ef6d597a6bf1dda9708fe38482b507c87
0x4d10812b09efa602caecb74019b15b065b340c0a
0x4db34e3cc4b77bc52bc8c9f8d79f6fdbeb53c47f
0xaadf2656026a7567564b43341dd5683e6ecc095f
0x3d2c3c74ce80b1d3393ff2f077e851304f663b51
0x87f72bfa1d838a9be5c0b81805a5053156aa5ed4
0xf98fe5618701726f99fc68b9f24574a23ff31694
```
<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/fa57a69a-0ecf-416a-ad99-3bb01786fe47)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9e2f6878-f30c-4bcf-b578-af619ef6028b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/98627949-182d-4265-b685-3045e3c5da33)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/41249b12-de4b-4d51-b9f9-a9d31c800258)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/38277bc6-7962-4104-bb7c-e5932dae8195)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3b81fdb4-820a-4fbb-8688-e328c9c76129)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/40d998ea-ea3a-4629-a438-c4b6e51e0841)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/dbd3e088-f4dc-4c96-9529-d9fc15ebea4a)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9dd9f0bb-82c6-46c9-8fff-aa224ab78304)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/22ee912f-c185-4b37-8e7d-7ee7e3b9de72)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c71a38d5-57ca-4bd2-b707-6ddf0e849b39)

</details>

Same TX, same amount, same day on all wallets. ZKSYNC farmer.

# CLUSTER 27

The first 20 addresses within the cluster are linked to the same Binance deposit address: 0x4568110400F275326A0d6DA0481F304bDf4551c6. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0x0a9c52dcce024dd72aafeb43c1c253b93ab6ee2c
0x810c3243032f3ac57e9351812f116c3ee6953c18
0x846e49ece01ac637f57c2fdf3effe476b7001190
0x8a1bdfdb9a6ba11dee57f7125bdd55ca54f651ea
0xb2aadf6bfc0a5213acb9c279394b46f50aea65a3
0xc27c64cde3635a30035817cc86b10d0104eb405e
0x26d125498742b99b521b838f31df87b22947dd5e
0x391891af67e29d97e61e30c3036a0874f5da411e
0x3e238207184db63b0883e8b63488173014a26165
0x0508fa31697d460e62bb918c7e08340fb2ff78a6
0x066b040ccdfd69e68eae78c2041da6e398b5d1d1
0x2138406a03f2b7e0daad86a8104625db598b6c63
0x2fa3479f42f38078943587f45d33a9bce36b23a7
0xd2a5b42bdde6d2ece36fc127540a419399057a88
0xb1e03d53f6be30c7154fdf5f125e7d713ecf722a
0x2253ef63addab1fab314e0d5e20116966b52d040
0x140f0d44991bf5ad752e12dea6087b46570fb8e5
0xbff79922fcbf93f9c30abb22322b271460c6bebb

```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/48ae13a0-7d58-4f63-9165-0ff742f3b7b1)


<details> 
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/248e4a92-46d6-4bb4-9760-5df9d7a9d7eb)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d3eef64f-494d-4186-9209-198427d1f375)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4e125b90-0ed2-4d91-a057-36675af7bfb9)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3cbfa482-9333-487f-aacc-0c8d3eaac89b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4b4a9ec5-183e-49a8-a5af-b7a0a1aafcd0)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/9191dad8-aa77-4b8d-8c15-99e5ec50518f)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/68f0c2e3-26d2-4a99-ba96-7a97eaf1a593)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/d2f1c0b0-e463-421c-a6c7-6a38240eaa0c)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/859f53bf-5c25-4eea-8e09-73f528f5632b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/95d43ecb-0b69-47d2-b27c-66e4a877bd36)



</details>
Manta farm that farming with several wallets the same week. Lot of fake positive but i filtered them


# CLUSTER 28
The first 20 addresses within the cluster are linked to the same Bybit deposit address: 0x4b02C1Fc0f39F03508BF62172d6b8D9C3D9910aD. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0x3c917b6223063c710287280563265ccaa71784dc
0x03de01e0cb2eb26274a0e35e5cb09a93f3a8068e
0xf01144cfa52420a23cb50fff509604587b5ba060
0xa2f25270e11c1f77b97e9d5ec63e1c01f7fcba1d
0xbdf1658f79eed4464fa97f92a3695ba81371210b
0xedc1f1bfc12385a730c808bd46364d5a2494442c
0xbf4f1b24b2639c9f71ca7f38b27cf385f1cec729
0x18c6702e6d871ca5b68e3f36196b4cae9a41e2d8
0xd021a881a3234f22cc95c26f23327a94327005c0
0xd4fe383e7d59c3e462866c62bda387cb6cd0609d
0x10fcee976fa1b3c374f13b60f00d6ac46c3a72a4
0xb79bb1abc006cb9f51b5bd5a35abae39e205c52c
0x5abb479a883b232f9a295d666cfa929e75ee157b
0x74ded6d821ac2423a729d797d15eb4c8bf7046ce
0x7dcd3037ac2b122af0acf6a0f1aa86859f7b9465
0xfe37afd03fa3bbdcd37e4edefa579dd9916c619a
0xceb3faacf0c0023cd18910ebfdebe620806e41d6
0x55c4c38449010ec12d1995ccbda727c691edc705
0x0415df1457856d4028f6391da5f5e1048e236cd0
0xa20eb2ee9b7551035cc4ce1d48e993f3c6b0d6c2
0xa6d9636619dac634badc3f2d4db205bbef991f02
0xe7bb7934b3551dcef122d6d4f6bbee8905817d10
0x549ef772ca4a50e2c8a416ae4121210d0ec5c52b
0x00ad69fe14ef5451c5ba4d307f7e326aa9cbe152
0x5eb51a30d56d0e023b46aa036be58cc12c16fef7
0xbe9eabd77e2b39c5dac4b8956e17ebb47fe94c44
0x4f47bc547d2743aca3886fcb1b7b5e011d46042c
0x0cac4bb9c939a71fb23613836bfa7f3bd4979c37
0x53814bb1808bbbd54d61b7c5cdf237bb82f03064
0x806fb45803d2fb2516305fc9a8a9e025110950b4
0xc64bf9ff387b1b0ae438118a80d82c00c54f70aa
0x715c0360eb98e1fbcf9482614ac2bd82bed1083b
0x818e74e32a0b511c3a76b9200e547fdf5a1f765a
0x9ca0e55b142efc4a2cff787880f1ce1508919d46





```
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/7c384196-9aa0-4663-a3df-b319a5864bec)

<details>
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/eae8e4ed-8942-490a-ad35-503d59df074b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/50ce82f4-1552-429b-a38d-5b187bb0cc74)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/12dc9a3f-27d6-4389-86a9-c0381cee7f2b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/3c5c965d-7548-416d-96d7-8a671fc8ea01)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/743b76fb-18c2-4326-97cc-70a224296487)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a80fe9ad-18fa-4677-ad39-f5b884dd2f8b)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f62670d5-6efd-4bd1-8924-5fd3e4f2b6a9)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f61b4032-3219-4ce4-b38a-7dbcbd5102f0)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ba39167c-71e6-4227-849d-ef5abebbfe52)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/45e31714-8524-49f3-84b8-1a1824564559)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/81744630-5746-46a3-ae59-972b1c95991d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6329fba5-2a91-47c6-a6bf-8306fd2d7ce7)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/79148840-4bff-42ab-be04-95a21ebaff70)
OP LOCK
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/6d9c64e3-1df9-44be-b836-0bda8b656330)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e5e27554-532f-4de7-889c-0c678a836b06)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/27f6a117-e90c-4016-bfe6-81832cf71163)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/68078f83-7916-43dd-a955-a6195f467f76)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/08ee4355-be2b-485e-a780-1f5aac7416a6)
ARB LOCK
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/b51a1b5f-038c-4210-9d77-42a4d1d12268)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/79dfb356-55b2-44e7-9ee8-01100c4edb52)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/76f20feb-357f-4ea8-a90d-338e9f199c6e)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/c12e2bbd-08b9-4003-a683-d143337acfef)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/ec30ee4f-f1fb-4083-aa4b-2670a56e5e10)
BSC LOCK
</details>
Sybil farming stargate via several chain. Caught.


# CLUSTER 29

The first 20 addresses within the cluster are linked to the same Okex deposit address: 0x39c6302662d84aF6E8a3F2B5Ed1593318663a061. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

```
0xd7a4ff75f082b0905e3c4b436b385ae2be61141e
0x82d40b38b4ec1380b0ee7c32a4682cb676b721f5
0x39c491cde3154ce63ec274d5dda1199af0d8ac69
0x8bfa806bae1ccde15be034725c88e6052f9885eb
0xbb1d382352150aff9dd2628905ee177410f5f587
0xa0a42bce72e4968e74a0d492b3f526c5ffb96f93
0x88f388a35429c42b1646052e5c528563a7457ccd
0xa84e8d582e33e4a0400d41f4d61566ae53895996
0x43c4ff80f884dd40bb5c0b9db62161c28390f91d
0xd48fe748c42abea4f149267900bd052b7614d903
0x3d29087b73e76f73978cf1c29a1f69ae31fc5c83
0x77b4f13d0d08c4bf4fb2cf960f02da1bcfc3d539
0x0bfd901dd7d89c20e30dc6f824a810c58c65d53f
0x28b5221cbdd6897dc8b8b72dd5433e5ebab36ccb
0x3079939d5e3b94c5decd71274a3a6f8f5df53c5b
0x760c5e4ed0dfeeac6c29084437a8eaa1eea68d13
0x86b961250bfdccd6d9077b6f34e1d24461675f93
0xf5f8e7d5791bf397c5e1708209e568671a7274af
0x30ee6df4faf455e27e275068d69c2540787fe161
0xad75fd76653d952f1ea5e02d551020078c8c07d6
0xaee15bdbcc2417e389eb4217fedd1ec3afd24f7f
0x19da959a377298be2198515da6748d121773c893
0x8cc54cd68f51bd6157f4934a210856361369bf52
0x443f5496ebd7fa04792a4d2ae92e493568173640
0x6a42ff25032d4a57a5ee2e0a902310643062e38c
0x01578b78e89bee2da3d7d55b531ad7b4c3ca80d9
0x579e2925f8b602c482b864e4bdfa79480a61e826
0x4a0683b791bb4831b93ec25acd8a8eeb2c70b1a3
0x5821d7dd09efe8736208e4dcb2a71fd32104f7a9
0xfcb1eb58a3165de8a8eac0de71beceee15d6a3d9
0xb50fbb1edd47f7cac09be31d7f36c44e7241a7af
0x9d5a128b83f0528365e5b666a279529d2e2a5062
0x7410ac97b15769c80eb68bbf21ceedda39b8cf3d
0x3e2b1a4d547dd3ed21feb6dba0972d9ff9e73358
0xb985ba1ae77fa3b11ad0f8e08178af0e44a49684
0x5a7c5585eedfb226df56031cd53cebcf82ae2a3b
0x2c49c4ac45bfc515fe2e7ea56e4fe53aa4710553
0xc4fb3efdbcb6301857ecf4f4990bb809970eb592
0x8ce69a5cd0d0ff3ea42a92ca0fe9908dddf6693e
0x4bae60d4f72b6b237a64337c81597f3fb24fa68c
0x41293d81ae5cac64744c9e6854f4473ead036261
0x8ee0a927024fa2c4ad0d92c1f083f28f643accc3
0x48f8a6a2860a7e9925fd458651e5a3095e8af88b
0x171cab023caa3ad62fedda04971f2c4c7d6f800c
0x21816e24a0d79f543c71c1113e5005521b429229
0x5b4eb77eec92d9887c6e0460c3ee55ca3cc78938
0x37ab23c4e27131aeee8584f8d0186711cd4cc2e5
0x5cec6821154dfce3348535d2815c6a9fc50e133d
0xd1f050038d4ae60a02d52e64a04b260ef57010ca
0x757be2c0996ded06e8ffd762d70f1615137772de
0x4d5f5471f7ba9b3943ead9720d4115c0669b99f0
0xbec9fd9217a3d7fa7c7e8778875ec78f9950584c
0x34137a3857ff4311ae800fc7c057397291dba601
0xaeedd4e25f74557f1d2e84ca12bcc9863c47c084
0xed97fefc8f8c4599a4d316c27e0775b9d45e1d0a
0x7ac1d0df59cb2a3509de6e1574b177f2dd4bafab
0xa695e1678d7d42c0dcbc751c52b1e91efcf16d8b
0x2c4b6cd8e01387efdda6e296c854bc627fa9b809
0x82076a79bb64b4927207d193dde11d7a089616d2
0x115f8974e7f6918d581bbf5bdea5993c60f8db4b
0xfe61acb7ed1020fd0bf1b2096d6ac3942c73228d
0x3f293d156a7371b580e25cdbbff0f0c5071f93b7
0xfc01e520a32bdb901b89533853fc25e7dcfd88be
0xfcc6a14243b44706f4bb4c1425de550d6b8af39c
0x1688438438aa95e53f11170aac3e267eaec947be
0xd86eda34aee5772c94fd53353f2938122e6f3220
0x9801036f66999c45fbc37b884e72d539897b8587
0xb984b6f567d76d29985404cae7593efb41011d41
0x6a406dd1c9d6f7651025b80b705195ae56942085
0x8454011a0ec0cbb62636b8723d529682cc0e51bd
0xdbd75ebe36bf769cee849cdb56f1599369654327
0xe8459137bfb5cd105ea2436bba652d76ea33e3ec
0xc73e35606ca7f296d37ce5564128b6352bdbeaf8
0x932585c306f13e7bfbb2a1d3ee623411e9839164
0x64a4bfe366c1172669cdd91c931141f0d4868b0d
0x134167a22c327e6badc29d3e230bcc08634f65dc
0x8b57322d54f67edb274b0bc6eb7a539dd804caf5
0xfad394421ab10af8957cd2ab7b066c236e4a6e5d
0xab10c6c7061da433c683a6be1728dbad6e836e96
0x88f388a35429c42b1646052e5c528563a7457ccd
0xbf418601b43143f30aea09bc1b1458fa89728dbe
0x013e7e29c34d560a5e0af584f7a6d879ef0f1d26
0x7abe177aff0232a31a2458e386d3a6a3229bb7c9
0xf735e3a90bbdfca9041d55dc6ed6567e731f5b1a
0x715214c9afdbf96cd86ed717c723c555ff1b37ee
0x6b01882f6bde7406efbbc783faca9f67c62b618e
0xcb328455981f19ff658fdca1249a553b083857aa
0x1cab98cf3b2a940d8077c95706d6ffaf01ced174
0xc85a30040cc062d600c7604c813d6981f90ffa15
0x0d5f869dfd7b9b7b02a3e50be490f9a6bfdf6880
0x814f217ef890220760e500db6a91ca9f2851db60
0x11ec588257425f46179888cc2224b447983ff5e6
0x8f484100d41d3820316e9ba1d5574e7eeb0a1d6c
0x7ce48915751a0dda26772b3ace54235a4186afb2
0xf3e1a7649731a15916b0775ae09d7809d91d8349
0x2aeb003a1568c39d8123d9c67acac1ad8931e6ec
0xab3c5e1501377b53ddd8020767ddc92900d263d7
0x2a6b24efc1c4ea30f052f0c89d395bc11977df1f
0x2b5b573208d59fc1aca26ac9d0d2a0e6ef49537a
0xce8bdca9cdc525099e60b192c0b88455acb2da92
0x7f2ed450425d7426c099e550df2b2c2b6bef1024
0xb16097d29e7d98e1de3a3dfc4120408c5a77e5bc
0x6494cee19a7b7d4a36af9c2ca8f20c70d07c17b5
0x7b5456114f4dac5d6b8319a93b637d5a87e6f584
0x0f36652574adf926018d6a34c2f152720a1ad758
0x39cd3f68fbcaec1790356e0a8df1d5b13531c2ed
0xe001c43e1188e0a84ed22081af46012411bc2028
0x154b5d681777cffb77e191618cbf5fe93346fbf7
0xd578247befc7d243e463383601ecc9393eeadd7d
0xf89b7092a1f744a19ab5304c1232e7798fab59ff

```

This one is a big Sybil that uses a script to make transactions, I made sure to leave all the evidence available for you to check too, you'll have to pay a lot of attention to this one given its size

<details>
  
**To begin with, we can see that he made batches of addresses which interacted with L0 on the same dates, all this information is on the Dune.**
  
<details>
  
![a1](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/2234b653-f92d-4550-86ca-c79102ae7603)
![a2](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/4ae9b674-0d41-41dd-8136-0d9ca9712c5a)
![a3](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/23c33127-4849-40c3-be02-c4316c485145)
![a4](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/24a91271-58bd-4e6e-94ea-b8ac69a3d14f)
![a5](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e37cff63-576f-4aa8-a63d-1a14fc34ad82)
![a6](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/47b29016-15be-4019-a3ba-00c0ecb5304f)
![a7](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/f2f3ccb2-067d-4f44-9c9f-a0fd66d585b1)


</details>

**He used his script to use the Linea bridge on Ethereum with exactly the same GasLimit (99301) and approximately the same amount (0.004x) between 08/23 and 08/26, then some addresses between 10/02 and 05 /10**
<details>
  
**I filtered out all the false positives
The columns correspond to: 
Address - Timestamp - Amount - Gas limit - Tx Hash**

![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/a4c4ba0f-da93-41d5-a97e-d7a698579acb)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/240f3b36-1acf-45dd-b048-d9b986bb07c5)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/804a8192-e0b4-447e-b8e9-5f3bb265034d)


1 0xd7a4ff75f082b0905e3c4b436b385ae2be61141e 2023-08-23   0.004253896656668   99301   0xca43e6011e118fa199c3601b4ccd80687ad1428c63c4d3b42002f9cd35cd36c5 //

7 0x8bfa806bae1ccde15be034725c88e6052f9885eb 2023-08-23   0.004716587160252   99301   0x7ab37a9532d97bfe18e6623bbebbbb5e98306de9dfd7d769962476e91ffeacb3 //

25 0x43c4ff80f884dd40bb5c0b9db62161c28390f91d 2023-08-23   0.004482017048988   99301   0x802b41b5866bafd7be9052a1deed3735ea841c2712e48dd0a3b313f3ff8433e4 /

54 0x579e2925f8b602c482b864e4bdfa79480a61e826 2023-08-23   0.00447298137282   99301   0x2f80b71f212b53d64c73b9c762c615ff7404480c67324dae3e10dcb50a995903 //

61 0x7410ac97b15769c80eb68bbf21ceedda39b8cf3d 2023-08-23   0.004691629688652   99301   0x920dd15a1fb37a7e26d34af61e27537d1f08e83ae9e033d093029277e621cd8c /

170 0x9801036f66999c45fbc37b884e72d539897b8587 2023-08-23   0.004475150301996   99301   0x70d47982dfb82cd7d74fd58f08a79e70fa5641b54ed9659b2b5770ecacaf8f46 

173 0xb984b6f567d76d29985404cae7593efb41011d41 2023-08-23   0.004742853059892   99301   0x6d0d135074c760437245f18206b1fb94ef5bff4b494be301fa60fd53a6ea7d05 

174 0x6a406dd1c9d6f7651025b80b705195ae56942085 2023-08-23   0.004655276382116   99301   0xf4d962b8935fa9deed576ef59b907edd0a9940eb161324fb40f1a030a1ae76ed 

175 0x8454011a0ec0cbb62636b8723d529682cc0e51bd 2023-08-23   0.004732399916028   99301   0x7aeeec81436d9ae47e94a983596c118efdc968c39b94d0222e5c2d7a783a583e 

14 0xbb1d382352150aff9dd2628905ee177410f5f587 2023-08-24   0.004192857422432   99301   0x5dcea627cdf047bdb32c9254017b7363aa8e25e5b12e5525381f6d7ad931e0d2 /

15 0xa0a42bce72e4968e74a0d492b3f526c5ffb96f93 2023-08-24   0.004243326647968   99301   0x5563159f1a44338132e1592ad11956f05c6fc137ae57a146a2e25b0f9d67dac0 /

16 0x88f388a35429c42b1646052e5c528563a7457ccd 2023-08-24   0.00424579059486   99319   0xd17e2407cac7fa3d08a048f4fc218627162856c09b9e1d7bf3384e4ace7a7a2f //

29 0xd48fe748c42abea4f149267900bd052b7614d903 2023-08-24   0.004337272878364   99301   0x703d936bc7479cfc80d2586c1872429dab957fe34618e75d943998b68f34a2c3 /

60 0x9d5a128b83f0528365e5b666a279529d2e2a5062 2023-08-24   0.004591626007068   99301   0xb93d22513c6a6f03cce74b6435a47510aed6cf91d96d621e672a20a345e5e75c /

4 0x82d40b38b4ec1380b0ee7c32a4682cb676b721f5 2023-08-25   0.004374759462188   99301   0xe81f49a1c1051f20d5aec9f64c2d8765339b10e4d931a8798297b68c00d66f11 //

6 0x39c491cde3154ce63ec274d5dda1199af0d8ac69 2023-08-25   0.004401930658496   99301   0xbd1a626b064191087bf6adb29075607c267f908318a9d6b23eb5c7a4cdde98ed //

22 0xa84e8d582e33e4a0400d41f4d61566ae53895996 2023-08-25   0.00448127457538   99301   0x3b1b52fb73d913e9d3f6fe8e35da521a642f6f314863a700472651375557599f //

31 0x3d29087b73e76f73978cf1c29a1f69ae31fc5c83 2023-08-26   0.004800648401064   99301   0xe1670f9ae7041c564da1980e95b31604a02ebed4fe759a4214dbc86b1abd71b5 /

33 0x77b4f13d0d08c4bf4fb2cf960f02da1bcfc3d539 2023-08-25   0.004749714895612   99301   0xd0eae5cc1913d6cf41fd8bcdcf2ef20082e30f2b2a893f3f0f076864862ecbe4 /

34 0x0bfd901dd7d89c20e30dc6f824a810c58c65d53f 2023-08-26   0.004726069661324   99301   0xc3c984e642168c106710d3866859ec10cbb39713e0274fc8cdaac8fe9d81183e /

35 0x28b5221cbdd6897dc8b8b72dd5433e5ebab36ccb 2023-08-25   0.004125486616252   99301   0x15c6e6d2973f93ed3fe2b7091854b571d7aafc837f4a7eab86101d2cda80f055 /

37 0x3079939d5e3b94c5decd71274a3a6f8f5df53c5b 2023-08-26   0.004429409740616   99301   0x5b31818a7cac018eb23a575bd32a1caff20d92f3a3a48bc53ac3004005e5777b /

38 0x760c5e4ed0dfeeac6c29084437a8eaa1eea68d13 2023-08-26   0.004841151657476   99301   0x6143a33e528d8818ec5adf195da6ea8b6015bf7715d7c015f0c2707696d8714c /

39 0x86b961250bfdccd6d9077b6f34e1d24461675f93 2023-08-25   0.004396798719868   99301   0xaa9b76968be0fa05b32bc5725295b4c233f75a79cb55eb7d9b4d2f889dbe46d5 /

41 0xf5f8e7d5791bf397c5e1708209e568671a7274af 2023-08-26   0.004892757994052   99301   0x3cdcc47f9128288634978a185d15c918de4948ccc02a04a51a4f384da669d5e2 /

42 0x30ee6df4faf455e27e275068d69c2540787fe161 2023-08-25   0.004475851628948   99301   0x1945471a4ed0d954684d9d3b40061b05b2076d2aa38935f316fb8722864b929f /

43 0xad75fd76653d952f1ea5e02d551020078c8c07d6 2023-08-25   0.004601259049764   99301   0xd6f51a918298028820dda66ef65eb563620ae5d6cf25b4de1b32786592d5da02 /

44 0xaee15bdbcc2417e389eb4217fedd1ec3afd24f7f 2023-08-26   0.004890477451964   99301   0x35cab4853f2e924dd19896ecb99d18364fdaa8259f7846d201511424c1116622 /

45 0x19da959a377298be2198515da6748d121773c893 2023-08-25   0.004462885765984   99301   0x6e4586db51948977bd22886164e286739bcf0dafd1ee2d514eb8196c66d933e3 /

46 0x8cc54cd68f51bd6157f4934a210856361369bf52 2023-08-25   0.004540426859308   99301   0x70160c922390dcca5fb781e12dac498e5c50fc04e3891301f0c4687136066b55 /

47 0x443f5496ebd7fa04792a4d2ae92e493568173640 2023-08-26   0.004788518803196   99301   0x74273f0633a6ed21489cf009d27692626db9c87f1a975eb51c6cd9a6cd5f3007 /

48 0x6a42ff25032d4a57a5ee2e0a902310643062e38c 2023-08-25   0.004168493842256   99301   0x3eced5ef34efc3d02c238dbe214c480d5b9f3bc962130fd642e27f5a020094e9 /

53 0x01578b78e89bee2da3d7d55b531ad7b4c3ca80d9 2023-08-26   0.004892560724236   99301   0xadabc246aa2a0aef05dfe49c79ae9493b7c6b12c635d468da9d5b875f969e67d /

55 0x4a0683b791bb4831b93ec25acd8a8eeb2c70b1a3 2023-08-25   0.004366157398948   99301   0xe317a7029876509cd1c4acaf64ee19edd1aa370e9ea90675f751fd60adeb32e5 /

56 0x5821d7dd09efe8736208e4dcb2a71fd32104f7a9 2023-08-25   0.004480010427224   99301   0x002b6c19764ca6e12351cdfc273e34539a9088c25c97afebf997e6e4bfb803a2 /

57 0xfcb1eb58a3165de8a8eac0de71beceee15d6a3d9 2023-08-26   0.00490511580456   99301   0x9df9cb293ecc3e1113a6d4b68bec53bcddf892a5c6d621977c27cb20fbd19a38 //

59 0xb50fbb1edd47f7cac09be31d7f36c44e7241a7af 2023-08-25   0.00444922257014   99301   0xe2025ea7543516502e919be8caf388f6cd4078d5b168c345525a13093dfaec5e //

62 0x3e2b1a4d547dd3ed21feb6dba0972d9ff9e73358 2023-08-25   0.00466348012882   99301   0xbb570bb99e26b9e57d191cce67f552ab08a270b860778211fd2d9ebc8d9b992a //

64 0xb985ba1ae77fa3b11ad0f8e08178af0e44a49684 2023-08-25   0.00445643618842   99301   0xf853d89bd01263b6ebca19b179822bfbcc931ef8e56e8c45ef59086ed94a253a //

66 0x5a7c5585eedfb226df56031cd53cebcf82ae2a3b 2023-08-26   0.004752784880248   99301   0x646a27967502a9c5a77f2ad22807ddb84511adce9b60a683f83edb3eb770331e /

68 0x2c49c4ac45bfc515fe2e7ea56e4fe53aa4710553 2023-08-26   0.004936111206888   99301   0x3f73258e649cf0543d8e46109639e67dfb540e2696492501097b87f479a26bb8 /

70 0xc4fb3efdbcb6301857ecf4f4990bb809970eb592 2023-08-26   0.004828999469524   99301   0xff54bfda8cec9fe90a5649ecb1aebc4841aa617ed023ffd8305c68a3a70e5d01 /

71 0x8ce69a5cd0d0ff3ea42a92ca0fe9908dddf6693e 2023-08-26   0.004901291562636   99301   0xc2f22cc8e634ed6eb318be59584a60ee488d5a0bfe58e2b98072f344fb0519bb /

73 0x4bae60d4f72b6b237a64337c81597f3fb24fa68c 2023-08-26   0.004805855859884   99301   0xc94afab9fe999d3d8d1dd4e8a35bd323aefbd4f7fc46424c9333eaad99f2636f /

75 0x41293d81ae5cac64744c9e6854f4473ead036261 2023-08-26   0.004799892166988   99301   0xb04b34de7de00004092a49a09787696b11d0dceec094d80ff0a242708ca02b25 /

76 0x8ee0a927024fa2c4ad0d92c1f083f28f643accc3 2023-08-26   0.004729557310636   99301   0x8316cdf120a6d71a7c28f717c48e5be5e4b5110ade610aced914a202dfd76c95 /

78 0x48f8a6a2860a7e9925fd458651e5a3095e8af88b 2023-08-26   0.004684532101076   99301   0xd0d9e34ea744cf31cc1dd41179f5f8ccec0491196d156cc4eeacaec52f111906 /

79 0x171cab023caa3ad62fedda04971f2c4c7d6f800c 2023-08-26   0.004664451831728   99301   0x5b1f615e9652d9f881711a68597264120b6d71844b7313f89bda445c1c94a15c /

81 0x21816e24a0d79f543c71c1113e5005521b429229 2023-08-26   0.004871725318452   99301   0x30aaa40f7b35bde805b1cdb1a4ffcf1bbd18c0aa44e5257053f55556d622b45f /

83 0x5b4eb77eec92d9887c6e0460c3ee55ca3cc78938 2023-08-26   0.004876637165532   99301   0x1537e1cbe2e64424cab552419adb728c069bef8fc1200520a3b7c96a408dbf0e /

86 0x37ab23c4e27131aeee8584f8d0186711cd4cc2e5 2023-08-26   0.004798269316076   99301   0x6bb91ab8227f79b764d6860bf4e8cfed9fcb4d36b96fbcb678fbebf2e580f1d1 /

89 0x5cec6821154dfce3348535d2815c6a9fc50e133d 2023-08-26   0.00479540123154   99301   0xb3e890b1a1203f573246d2ffb49ae21739d758af9378fa3d564f5314f81af5bd //

90 0xd1f050038d4ae60a02d52e64a04b260ef57010ca 2023-08-26   0.004887630723816   99301   0x217c7a709f39c3c6be716e48d5a97db981d7df9fc76141677f4f7f3787f082f1 /

92 0x757be2c0996ded06e8ffd762d70f1615137772de 2023-08-26   0.004768339061964   99301   0x80e9ee1947d202ab946659e21211f4d133b525f780e14a08cf242bd0a98922aa /

93 0x4d5f5471f7ba9b3943ead9720d4115c0669b99f0 2023-08-26   0.00477299853852   99301   0x2a79242320972b8fcc17142c8fe3671a7a54a63e64c0e70502e078d586b1a7e0 //

94 0xbec9fd9217a3d7fa7c7e8778875ec78f9950584c 2023-08-26   0.00473208101206   99301   0x5230b2dc115ca87f1013c45c363bd3800c05961d9f29385afd54237d6cf7fe11 //

105 0x34137a3857ff4311ae800fc7c057397291dba601 2023-08-26   0.004763543499284   99301   0xeab1b968776d14f3a71ab2b1356e6385e7d8d1811f345ed8f14ec1877559e2e6 

106 0xaeedd4e25f74557f1d2e84ca12bcc9863c47c084 2023-08-26   0.00487866054618   99301   0x043f9030adaa4a7bbd0553f6a427a94880fdc00e167ebd866a97268a51029b20 /

107 0xed97fefc8f8c4599a4d316c27e0775b9d45e1d0a 2023-08-26   0.004663888987628   99301   0x61b3647477f209e34d2fb6c00894efcdb6d54f1dd5cf63d6b3be26d6408d1594 

108 0x7ac1d0df59cb2a3509de6e1574b177f2dd4bafab 2023-08-26   0.004843443213956   99301   0x4399af15c39139392f5c3248cca6d39522185dabe837c4af2df15c12faf933d9 

109 0xa695e1678d7d42c0dcbc751c52b1e91efcf16d8b 2023-08-26   0.004864047174184   99301   0xda4b3e5d8e21135e92deb30daddabe0ff1bcfccd6a503bfca70e4ada2a3bd006 

111 0x2c4b6cd8e01387efdda6e296c854bc627fa9b809 2023-08-26   0.004816722086516   99301   0x77794a46d1aefa602b4b352a9b0913285e1b447f2ed902214485e98f722d82f3 

114 0x82076a79bb64b4927207d193dde11d7a089616d2 2023-08-26   0.004788792331244   99301   0x4afe132b24fbc5ac1cb4fe9b00d3fe2d783e5e350e7475eece6e8afb86b290b1 

115 0x115f8974e7f6918d581bbf5bdea5993c60f8db4b 2023-08-26   0.004899749314508   99301   0xe78b7baa44ef263f3f3ac684ef95beecd30283020abe24e21764a707baf4a17f 

117 0xfe61acb7ed1020fd0bf1b2096d6ac3942c73228d 2023-08-26   0.004861555128388   99301   0x08da0699d4c26a42788ecd92058bb2f397ceee91d91384534cf1edd70d875883 

127 0x3f293d156a7371b580e25cdbbff0f0c5071f93b7 2023-08-26   0.004706035724076   99301   0x88daf6bb49b065f5383684765c10602ca495918d6db6f647954f2a4992dd5d88 

143 0xfc01e520a32bdb901b89533853fc25e7dcfd88be 2023-08-26   0.004601691329764   99301   0x81de062f6987a8f64744ea488f6f872371b2ad810f27f894a2009858ed6b078b 

154 0xfcc6a14243b44706f4bb4c1425de550d6b8af39c 2023-08-26   0.00479864319334   99301   0xe8a82e97b6cc15fbe5af85eccf649cc8703279d5623562110d930872c0b44c52 /

155 0x1688438438aa95e53f11170aac3e267eaec947be 2023-08-26   0.004798738251172   99301   0xc4e56a173c907eab29d400c7d9fe762b402f5711f067cba88ae5627ece9b5313 

157 0xd86eda34aee5772c94fd53353f2938122e6f3220 2023-08-26   0.004895398972604   99301   0xcc0817215a488feefeeb50308afb31e252a2ef49a32c15092dd76cab0a15333a 

18 0xdbd75ebe36bf769cee849cdb56f1599369654327 2023-10-02   0.005112448167408   99301   0x203223f40e96d44a2b4f9ee424399660413f6673d5297316a765f3988ea64e5c /

19 0xe8459137bfb5cd105ea2436bba652d76ea33e3ec 2023-10-02   0.0051122375223   99301   0x8350c9f59f30e48d58d69f537bc302955ee8b632980c485c846d00becd817cc4 // 

20 0xc73e35606ca7f296d37ce5564128b6352bdbeaf8 2023-10-02   0.005112448167408   99301   0xcd3b81b16c26127e7c6f173fd4f8b6cd3ae1c6cfdabd94022f165f6f03e8f9d2 /

13 0x932585c306f13e7bfbb2a1d3ee623411e9839164 2023-10-02   0.00444225004854   99301   0x7746c1886223687a8e8c909b1839d4f3aea6eecf4b2a37a7aa996df8725b09f5 //

51 0x64a4bfe366c1172669cdd91c931141f0d4868b0d 2023-10-02   0.0051348018642   99301   0x4367a3d43b552968ec96b0ac6e89ec892747aa5bc0ffe709d97895c603c8c612 //
65 0x134167a22c327e6badc29d3e230bcc08634f65dc 2023-10-05   0.005605801125768   99301   0x52f685e49476a9784a80febe539d8c003b152985d5c572c0e5ef05b8b6e2968a /

3 0x8b57322d54f67edb274b0bc6eb7a539dd804caf5 2023-10-02   0.004112556868076   99301   0x310735918b1676d003f141906f3d9b289e17d7ac188c5945052c3e97e0f8651b //

</details>

**He used his script to use the ZkSync bridge on Ethereum with exactly the same GasLimit (149293) and approximately the same amount (0.007x) between 08/31 and 09/26**

<details>
**I filtered out all the false positives
The columns correspond to: 
Address - Timestamp - Amount - Gas limit - Tx Hash**
  
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/460ee20c-3c80-4d41-b836-7cef80a9c6c2)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/e666cb69-5f56-4621-8164-287cf29a944d)
![image](https://github.com/bigleesnitchin/LZ-Sybil-Reports/assets/169681941/da4b3852-cdfd-4c4d-b6f5-6c2b8cd0a1c0)


2 0xfad394421ab10af8957cd2ab7b066c236e4a6e5d 2023-08-31   0.007882454   149293   0xc7054b5bc0c56dc6c9a0a1c7d346141c6a28d5d2c3a91e848e0a13dfecbcdb15 //  

4 0x82d40b38b4ec1380b0ee7c32a4682cb676b721f5 2023-08-31   0.007836454   149293   0xc016e3e5855c9a52133704bf5409576645060ebd8dbd34717478695572b9859f //

5 0xab10c6c7061da433c683a6be1728dbad6e836e96 2023-08-31   0.007662454   149293   0x3b53061544339f3cecb0fe49a86e6a7cb4fe91c95bf89c231a5b905170db7853 // 

6 0x39c491cde3154ce63ec274d5dda1199af0d8ac69 2023-08-31   0.007812454   149293   0x9dcfe1beb4f1203e987685f7f18e5e43794826f2d94807d910892c9055f33d75 // 

22 0xa84e8d582e33e4a0400d41f4d61566ae53895996 2023-08-31   0.007722579453533176   149293   0xa700e0a86646b36a2e9dd3867b0dd3feed45a59dc8a6ee10e4c1f9af98c6defd // 

32 0x0d5f869dfd7b9b7b02a3e50be490f9a6bfdf6880 2023-08-31   0.007912454   149293   0xfc7687cf33c89cbaf1b195ace4ac80b227c4458efc00f4ee67742a1f43617ad3 // 

35 0x28b5221cbdd6897dc8b8b72dd5433e5ebab36ccb 2023-08-31   0.007783454   149293   0xfc5b50edd6d041d476b10b50eb71bd0615a7e010e1858ea6aa0b059566bf3e9f // 

40 0x6b01882f6bde7406efbbc783faca9f67c62b618e 2023-08-31   0.006797654   149293   0x209fad04f2eebd37ada8e64869d4ddba5e377794b68f729b6f4b977d6248d1da // 

42 0x30ee6df4faf455e27e275068d69c2540787fe161 2023-08-31   0.00741478732433888   149293   0x7ea04c08e127e59e7e20d7f39b86f7b760c60a5f5acc56924174ac2003fcfa07 // 

45 0x19da959a377298be2198515da6748d121773c893 2023-08-31   0.007762454   149293   0x89365b5be8c40a44e12e8398ba589be1c2a03ea9f3464a5012b69601c2bb00a8 // 

49 0x11ec588257425f46179888cc2224b447983ff5e6 2023-08-31   0.00757856371028402   149293   0xc74a6a25beb4e88e16e76c0e484b1b6dbc59563ff93fac4c26366efc528523af //

55 0x4a0683b791bb4831b93ec25acd8a8eeb2c70b1a3 2023-08-31   0.007368158089030436   149293   0xf28287bc4b16e0a3f2c47ef3501a780173ef6535a20475c21b6aa2d5beff6ec6 // 

56 0x5821d7dd09efe8736208e4dcb2a71fd32104f7a9 2023-08-31   0.007404485187519096   149293   0xed7cbcc6d24ec07679f03a2eb68cf3620ea4b4560991ca4870c10dd98d782d75 //

59 0xb50fbb1edd47f7cac09be31d7f36c44e7241a7af 2023-08-31   0.007611454   149293   0x1fc68f85c42d15e88aeba16d586280913c907b2f2cb66cddfa73f926f808d673 //

60 0x9d5a128b83f0528365e5b666a279529d2e2a5062 2023-08-31   0.00752670516164326   149293   0xfc7786116bafc32ec024750030448e638fc151b56941edceb667b43f7a4241c8 // 

62 0x3e2b1a4d547dd3ed21feb6dba0972d9ff9e73358 2023-08-31   0.007781454   149293   0xb6bab3d876134dc571a0b88bf7c06edbaaa7ddc6c00bbc1e76e72c7758e3508f //

63 0xcb328455981f19ff658fdca1249a553b083857aa 2023-08-31   0.008092454   149293   0xaa8256ffa07a1eefc2c4221577a51f29270f3a37ebc93d4f4938a1cf143c1cf8 // 

64 0xb985ba1ae77fa3b11ad0f8e08178af0e44a49684 2023-08-31   0.007427239786617848   149293   0xf6d91fdb1300a29c4fc35919c2cf0b39d4664d3cd2cb5f85c0170bdc749a3e50 //

67 0xf3e1a7649731a15916b0775ae09d7809d91d8349 2023-08-31   0.008001454   149293   0xb761b8d3ed685cc3ef72fea90581d1a77f197f287db3fd8066e060742099e0b6 // 

72 0x1cab98cf3b2a940d8077c95706d6ffaf01ced174 2023-08-31   0.007810454   149293   0xb393312056fa0c8deddb385b2c085ac41d67a6e7fc86e6651f713f66546cd02f // 

31 0x3d29087b73e76f73978cf1c29a1f69ae31fc5c83 2023-09-01   0.008481454   149293   0x7f0fcd224932d846fea8827a0ca3145f8fb24bea3b672d282c018b7a23c52d6a // 

33 0x77b4f13d0d08c4bf4fb2cf960f02da1bcfc3d539 2023-09-01   0.008364454   149293   0x039a8ac855ef9157979f767ca52e5561dbc1c712ff4cebe67593e78b4504495a // 

34 0x0bfd901dd7d89c20e30dc6f824a810c58c65d53f 2023-09-01   0.008181454   149293   0x206c4a2906c52aa57db550476e29ab956b2984b942265ae404d9df9a4c59a47e // 

37 0x3079939d5e3b94c5decd71274a3a6f8f5df53c5b 2023-09-01   0.008031454   149293   0x956751d23ed348925260eda3a16f8cb3ad609f3c7e2d7feece71b1268ebef3b8 // 

38 0x760c5e4ed0dfeeac6c29084437a8eaa1eea68d13 2023-09-01   0.008351454   149293   0x386b1d207570d01d1172603e4a8fcd1e0946fa22a8b9a216a835e5a24a06c25c // 

39 0x86b961250bfdccd6d9077b6f34e1d24461675f93 2023-09-01   0.008249454   149293   0x2e0c10e125eb481127a82315d1f17d972f5ce3f88cda42248ca228e0accd66ef // 

41 0xf5f8e7d5791bf397c5e1708209e568671a7274af 2023-09-01   0.008581454   149293   0xd7b32d049d744e5cd6a724262f9dc4bde0647be07825648db9f7156ab46323f0 //

43 0xad75fd76653d952f1ea5e02d551020078c8c07d6 2023-09-01   0.008334454   149293   0xee4aacecef2ce2739319862c937f29570d64a9ff3df2767b3b65ab8a3d737215 // 

44 0xaee15bdbcc2417e389eb4217fedd1ec3afd24f7f 2023-09-01   0.008181454   149293   0x392d053796a5117693e4be8893eb73af5cdda57712723e9d61dd7a0f36a4ce54 //

46 0x8cc54cd68f51bd6157f4934a210856361369bf52 2023-09-01   0.008070454   149293   0xf97042f8b555e4f0cc6fe0719d22b3e66db77a9a1961f67fe79dbd6d31bfd44d //

47 0x443f5496ebd7fa04792a4d2ae92e493568173640 2023-09-01   0.008381454   149293   0xfd793f1375d4f00cdd1c6ac75b9c2bccaa4e76038492743f63908ac6c6cdfee4 //

48 0x6a42ff25032d4a57a5ee2e0a902310643062e38c 2023-09-01   0.008309454   149293   0x90bece7e0529a36b3d74cbb5e5b641c5bdf49fcd806a7047ae90b32899d6d1b5 //

53 0x01578b78e89bee2da3d7d55b531ad7b4c3ca80d9 2023-09-01   0.008681454   149293   0xf953aa6ef3fbc1e17facb1308655c3e3b3a410c66c807051132fc9904987ba1d //

66 0x5a7c5585eedfb226df56031cd53cebcf82ae2a3b 2023-09-01   0.008381454   149293   0x253b50cdf004d3dfc0e1ad5be84d762d2a97b704d78a236d11ccda966fb0d3d3 // 

68 0x2c49c4ac45bfc515fe2e7ea56e4fe53aa4710553 2023-09-01   0.007581454   149293   0x4c1d41f86cec83a6e21d1904733fa1a0b306a77875ca591575233f40dc1f1445 // 

70 0xc4fb3efdbcb6301857ecf4f4990bb809970eb592 2023-09-01   0.008281454   149293   0x240ee512fb066b35148423981bc24877908d167525bbd04a3c88dd6aeade3b5d // 

71 0x8ce69a5cd0d0ff3ea42a92ca0fe9908dddf6693e 2023-09-01   0.008292754   149293   0x86a76896e3dafd1f758d2f18f834efb50842f65a1fdade22cd8bc0bf9a7d00c5 // 

73 0x4bae60d4f72b6b237a64337c81597f3fb24fa68c 2023-09-01   0.008331654   149293   0x72165cb8912333829863eacbb9e0ff618830aea4e8c046a618575683da4673e9 // 

75 0x41293d81ae5cac64744c9e6854f4473ead036261 2023-09-01   0.008481454   149293   0xa0e139c18496d57f1803645176ecf9d2f520ac8640e0d74475f8eac2f6e8f8ca // 

76 0x8ee0a927024fa2c4ad0d92c1f083f28f643accc3 2023-09-01   0.008281454   149293   0xe29b4cc193be725f9a6814d1db92543f37a7e2a2e65e1d3893a8594d4f920d76 // 

77 0x2a6b24efc1c4ea30f052f0c89d395bc11977df1f 2023-09-04   0.008400154   149293   0xf873ea2dc0a924ac4e3fb6b5a51b3fd752887e8b844539e69f5e55181c9251e6 // 

78 0x48f8a6a2860a7e9925fd458651e5a3095e8af88b 2023-09-04   0.008402954   149293   0x1a7678f8072f173cabcb1e9645d4d08f5a194da7cedb8840842f6c6401aba4f6 // 

79 0x171cab023caa3ad62fedda04971f2c4c7d6f800c 2023-09-04   0.008623454   149293   0x3bf9c4c767254d747090c2a4a4ced18fe8817e6cdb00d24459e35673b354c852 // 

81 0x21816e24a0d79f543c71c1113e5005521b429229 2023-09-04   0.008604454   149293   0xf8d3b13021ac7fbdaed323ec4902646026d4c1380fd7a5efc910fd22abbeb975 // 

83 0x5b4eb77eec92d9887c6e0460c3ee55ca3cc78938 2023-09-04   0.008612454   149293   0x8992f03476bb448c40d48d29d685766ce936f82a5f270d136abd40c9dcf6921c // 

86 0x37ab23c4e27131aeee8584f8d0186711cd4cc2e5 2023-09-04   0.008559454   149293   0x8c4f648d6c49a911a7534c124df24690a3f24edb510ea1558314665f444aa4de // 

92 0x757be2c0996ded06e8ffd762d70f1615137772de 2023-09-04   0.007294854   149293   0x64e3c82cb76c669b982372d7589e7a9c8dc3b567bfb0a36d4090d6eb677346f3 // 

94 0xbec9fd9217a3d7fa7c7e8778875ec78f9950584c 2023-09-04   0.008312854   149293   0xf72fe1b76944a8c34b39bc4df3a021cf143383e89ad8efe1396fe977bafbb353 // 

111 0x2c4b6cd8e01387efdda6e296c854bc627fa9b809 2023-09-04   0.008595554   149293   0xf20a8d1922f93557bb5767c036035882a62992c05f867c7a57b94ce70007cead // 

127 0x3f293d156a7371b580e25cdbbff0f0c5071f93b7 2023-09-04   0.008528054   149293   0x46221949e9cdfb165aa8c095746f1228ce8b1c462d51f13e40eb631ad230d7fe // 

132 0xb16097d29e7d98e1de3a3dfc4120408c5a77e5bc 2023-09-04   0.008565854   149293   0x3d864e86654931edc977bea02f2d55afcae99b5ba0fb1eaaa799f55a5c37430a // 

143 0xfc01e520a32bdb901b89533853fc25e7dcfd88be 2023-09-04   0.008381454   149293   0x57ef00c17ecf36e5deae4ef85c56c177ff305facd83c969fd52e6abfad366647 //

143 0xfc01e520a32bdb901b89533853fc25e7dcfd88be 2023-09-04   0.008381454   149293   0x57ef00c17ecf36e5deae4ef85c56c177ff305facd83c969fd52e6abfad366647 // 

57 0xfcb1eb58a3165de8a8eac0de71beceee15d6a3d9 2023-09-25   0.004987467   149293   0xcdd2f7f37cb71a73731f65da7e379c94f2f342055e8bc08d83a637edced8e274 // 

89 0x5cec6821154dfce3348535d2815c6a9fc50e133d 2023-09-25   0.004986907   149293   0xef2ea3472ac9ccf521822307fabacdf691cb473467201c54c03ab991e39f83ae // 

90 0xd1f050038d4ae60a02d52e64a04b260ef57010ca 2023-09-25   0.0049870935   149293   0x5946dd20daad5d6f23816b1d572335afba0c93ea888b2624fea823f8e64eb4ba // 

91 0x2b5b573208d59fc1aca26ac9d0d2a0e6ef49537a 2023-09-25   0.004987654   149293   0x5c4355ba0f63c4e1b681f0b1700ff226721389ffecf63fda7e0190d56a58ad1a // 

93 0x4d5f5471f7ba9b3943ead9720d4115c0669b99f0 2023-09-25   0.004986467   149293   0x976bd113f3df125b20d487812ba421af58302029c8582f4592fc79c5460dd001 // 

95 0x675e49cfe9a76d8420dd15f9f5cb3fa5fe37a6ee 2023-09-25   0.004487654   149293   0x3aac8b631fa9063561b2d031b7c568553d3ab67cb852d7d378cb25308ca9c0ff // 

96 0xebbf5fda701ef5bc1591e90f7fe6db5450e6da71 2023-09-25   0.004520104   149293   0x404ab951589254037a3bdc03ca734a0095f83a88bcfa0c9e64694d8b75e9d22e // 

97 0x6045eeede3ce66922cbe215b6de01cd15bd8438f 2023-09-25   0.003887654   149293   0x884ec2d0520ef85f5b75a2aba6134cd7ac2e6151e5102cb6c284fdd400d4df8c // 

100 0xedde9378deb409703fdb18b4da413785372d1964 2023-09-25   0.004276617434113641   149293   0x6242a4458e922e289058faf4254485578b0c961bbd39951b1eda27e51fbfedac // 

101 0x889728a3d109e561148a378b5914d0ebcdb4dcb0 2023-09-25   0.004424885436656435   149293   0x9140f3c6af727a059ea0f855642d7d02701019e9a6b4801b8c615a7a886581e8 // 

102 0x75e7d36b6898f25ea75a05f7fbde5ed63877e474 2023-09-25   0.004301179049946897   149293   0x4b94e4a7810ee8976a734c7ee45e32f9980eeb04f16cdc8b7ca2a6a734d69999 // 

103 0xf5aec6207c55c9ea23864ce66dd954ec4bc53436 2023-09-25   0.004594051827063335   149293   0xbb48f6a48e15ffba3b316b2e6fc05f5461b90dc63f25b6c0ea68d7f754cd653a // 

104 0xe9c8efc1ed3de36175a4902df743e80de2b848bc 2023-09-25   0.004169361958596631   149293   0x74fe7b0992397d496899e2a09f64b0985b822e588385f89025544168139b178a // 

105 0x34137a3857ff4311ae800fc7c057397291dba601 2023-09-25   0.004988774   149293   0x019a4423105ab7ad831bba136dec2e7e90188d5608b5e8d21a4219cc72ff78be // 

106 0xaeedd4e25f74557f1d2e84ca12bcc9863c47c084 2023-09-25   0.004988774   149293   0xaf195e181044790405a99f3fc6d85ef9df42bdb783af0e07e388c00a94f54684 // 

107 0xed97fefc8f8c4599a4d316c27e0775b9d45e1d0a 2023-09-25   0.004988774   149293   0x386cc0dc2a5ada4848415ff6cea2d693a11ae07c87b9670d3c519630ad015c96 // 

108 0x7ac1d0df59cb2a3509de6e1574b177f2dd4bafab 2023-09-25   0.004987467   149293   0x62b6c982d4ea552124992552de7b2efbb9d0a575e97d337f3349d6edfc0732be // 

109 0xa695e1678d7d42c0dcbc751c52b1e91efcf16d8b 2023-09-25   0.004987467   149293   0x06111e616a11a562dca6b7c32cc813bb09e9fe3b989c5b0e660b49dbfbf8755c // 

112 0x231450363df0e2ef240e54f14ec02f957160e484 2023-09-25   0.003191626   149293   0x5eb223815183b1e5b9b50a694bdc13255bc11ddc67182c6d6a5ee17153052367 // 

113 0xce8bdca9cdc525099e60b192c0b88455acb2da92 2023-09-25   0.0049870935   149293   0x2ba91ba9ce20e859f7804f989b6754b53713dff4eec0f7b38c8362e955621e64 // 

114 0x82076a79bb64b4927207d193dde11d7a089616d2 2023-09-25   0.0049870935   149293   0x38f0092f3a29334a45cafe1cb155af69394df042785774bcff81c7903fae3980 // 

115 0x115f8974e7f6918d581bbf5bdea5993c60f8db4b 2023-09-25   0.0049870935   149293   0xfc01e0b2c9eeda3492a86fefe44580a2439733a68999ee626641f641b3f7324f // 

116 0x7f2ed450425d7426c099e550df2b2c2b6bef1024 2023-09-25   0.0049870935   149293   0xbe5801b5b13106b93b8809a51f5fea96060b56c536e49b1a8c892235e3fc22c3 // 

117 0xfe61acb7ed1020fd0bf1b2096d6ac3942c73228d 2023-09-25   0.004988774   149293   0x77e7a1b2bf387404bb1554c138fbb75885244c99e3760af926ebcb1382d9d032 // 

118 0xc245c38a27050dfb45de5b8d92e1c838c38b5943 2023-09-25   0.003541626   149293   0x13abc37133fa5eaf5364f3eac904b14418af7fdffa8d98818e980a26d97a9bc1 // 

119 0xb4fc4f8a9a998324822dfb2ac8359477392f4b79 2023-09-25   0.003491626   149293   0xbfe8196277140cbc5b5b757d2f1784d397c4fdb0633c7a134fba09594c009081 // 

120 0xdacd7fe0d229adcdad3aa2b645a8f231d42b66b1 2023-09-25   0.004191626   149293   0xab867eaacaa9e59632cd9c7d154b816eeb3c5c06c9a029f3b3bcc4bcb6b90d4c // 

121 0x6aa9d47f6e239d53094f3890b3791747e98d18c4 2023-09-25   0.003891626   149293   0x4422621ae71be60965c3c677bc12c909e472dc7743b85b8c774e66450e0bc206 // 

122 0x76ee6dfc1d027227e24186c3f12cdb4541cf5e9d 2023-09-25   0.003640368   149293   0xb785e048f54a91a8677867c851964b30129a8e39e5262f4f20864c1410478e18 // 

123 0x1203a593374b3c55ce639ffefb7b49ac3cef9622 2023-09-25   0.0040903415   149293   0x3bb6592855bc9e46de9143d8e6447e64a8db92320294d82341c771c8c65fa973 // 

124 0x55148a5c549fd20e42b4cc4017542b1f2a6fb46e 2023-09-25   0.004138157   149293   0x7e624040545f8eded7a69045497da35edaa486592d653c9b21ac341606c84e64 // 

125 0x97eb69f8bdca46ee57abdceb82098ebd01411560 2023-09-25   0.004039067   149293   0x90169bd511ad12f43cde27eeff73ba74d8e9d19ad10a0eda9123815dfcbc7f20 // 

126 0xada733154d7c9750b0d3e117c5caf7f7661f0267 2023-09-25   0.003486774   149293   0xede0d4c840e17ea1a88702c9a7322d1c8d5195dccc04852a0b9e52fc6d72a7a6 // 

128 0x32d796eacdabe6ed6f4f37f1beedce1056a217fc 2023-09-25   0.004138339   149293   0x2235451ccda863ba0cef034847276bd81485e433e117a31214463e98e32ab836 // 

129 0x2f15e0275a332590e77591bfd53168d9c2d4ea96 2023-09-25   0.003687429   149293   0x6729e4d450b64625750f05704454621aebedbddeea9e02d702361d41f8d1bf88 // 

130 0x9b897c66dde3fa2a845ddbbaa7448936264fa6be 2023-09-25   0.003887611   149293   0xdb8834fd12f78f86fe71f0a77c6e12a2ee02cddb275d3b1961c580462511455b // 

133 0x5f4f213fc8c085e5a2e31f08eae1fb074febf44f 2023-09-25   0.0037910695   149293   0x48569e80b54de02d665b4423938c12335294a0ac6bd560a5b57a2d9e28427d64 // 

134 0x078866c065feadc9e0be285d7dda8fe39cd605e2 2023-09-25   0.003782089934456668   149293   0x8cab4ceb9de6ed8db5d052f05ffd7d34bc829ac7d6567fa31ec8211aacb5aa34 // 

136 0x5d0e820d2be3b2b951416f5576978fca7591b610 2023-09-25   0.003560096345613869   149293   0x9ac34faf9c43960d5c3635db47e47f771929be3ff920c522df8a57a3c974cb27 // 

138 0x741e5b6b5e802c46f815c4dd4f5de7d89efa9032 2023-09-25   0.003589795   149293   0x716d0bdac6a66ef933590b2d2accef611f1ff3eafc99f22fd40f1bce91b1926f // 

139 0xe3bab6a9c6197c9fe34ec4d67f92bf815d9224f2 2023-09-25   0.003648339   149293   0x54a2cdab42453e8c25be455259353ac515e9a623b27cc2d27c2ba3a5018e8a9b // 

140 0xac5c7f8f0e69beb0892c59c93d67afe742b3ec74 2023-09-25   0.00363262154692344   149293   0xf66b30ff5f4ab9bb30cc67b8b6277af85d688ce011b5e9e088eadb2b9dcd231b // 

147 0x4a6ea370cfd5c2343bab414872eb988846adfc44 2023-09-25   0.003745683659868904   149293   0xddd531c76506280ac42ef9c9cdf0e9e7bed27d77660503931586b3b625409549 // 

148 0x3f81a8be0bcd8954ff05193079ac3e6630be4660 2023-09-25   0.004096097310912437   149293   0xde2fa36dbf7bb23bb1bc3b1eb978f9fccb7f73dd051073c450514bba86f18aea // 

150 0x730be13639b196557f223039575b1c4ff4e723b2 2023-09-25   0.003902192649872106   149293   0x03df9ed96c6c50e6a1d749edf5f5d5754f2ce5585d5c42a80fcd24617d4b5edb // 

155 0x1688438438aa95e53f11170aac3e267eaec947be 2023-09-25   0.0049872805   149293   0x172f2ce733bcbf67b77e3b54a69ad9d133d9d56965415a205b2ffc844fe19839 // 

157 0xd86eda34aee5772c94fd53353f2938122e6f3220 2023-09-25   0.004988027   149293   0x2fc0df74b96b585f60acd368eb1e259510d03c043c47eee25e00ccfb9bc38c63 // 

80 0xa58a6092f7a16ba936a14c7f1b58cc406299ab69 2023-09-26   0.00438963   149293   0xf79de3f97edd2414e3545c02eb094001c0f0f65e1dcc6423814f7babbf0adb01 // 

82 0x9de2bdad097efc4c92dc30b2cd1b80fe343a0fa2 2023-09-26   0.002491626   149293   0x20e634d2d129fdf970bbd81377d0237309d0f55e7401b80d61c978cdd44c2960 // 

84 0x97bfb4975d9483fc64bfe85acd7e14495e6c1ec1 2023-09-26   0.003991626   149293   0xdc8a96a2077f2786f7316d8eef950983f0534f1fa58a8bb21dc4f6490066ead9 // 

85 0xf652338727394f78d9cff1ad764db321e77c5fff 2023-09-26   0.004389334   149293   0x5297c5c691def4d61c48250d0f67b1cadaca17f06befe3dc217aa2bfbd50744e // 

87 0xbc442de7fe21082e03775e8c7ef4e5c1ccbd5b11 2023-09-26   0.0044889605   149293   0x638eb8b110d14ef119c8a175ccea9d5dbfd686fcb69b54d2edbb695ecf8092fa // 

88 0x7498f6b0040ed2045e7a2843a66f31bb1629c81d 2023-09-26   0.004228950047100456   149293   0x50dcbeb3f20bd9c82ad1a7d9bcd17e937d6de37cce90922df9f6c9b8f2d333f0 // 

99 0x51a95d8af4dd7a504b33dba9f67fe06579f02ed7 2023-09-26   0.003769291452822188   149293   0x60e72552ce382d709061bb09f8cec013ee44e766197a4c631892af2065cba65d // 

110 0xbed70d7f0ca7e9e8b8c470d1b2fcc99c74b33b80 2023-09-26   0.003872236218076761   149293   0xf293ac64b6fd93a884ab65a4a698e2d727de733e4c9a12cea33b6245bc8bf91d // 

131 0xf43c2d21b060d825ea2a15a55c0be3ec643b176a 2023-09-26   0.004508847089226439   149293   0xe0c93c4bb2e187d2e1d9794d35e21058e50d67b7af2c9cd51218dba32ff06cda // 

135 0x095c2643b0c04c3f9afe428baee97a98cc34907c 2023-09-26   0.003951403310024696   149293   0x18541b35248ca25e152f9a57a06b0dc2ffe6b287f26b399f69c8a4b137e425ae // 

137 0x63419c1b91ebdf5247c1a7edb66fae5aa2f931a6 2023-09-26   0.004227654   149293   0xd261e1bdfe5b47639c3242fc57707a664c74a5cd508374aae1d7c7c38b0a0e18 // 

141 0x5bb6e0d6cf5fb8b126e441fbef884e78df91adc0 2023-09-26   0.0042910145   149293   0xb5d833429879796b69a298556b8e3186a6d0a78ecd8d213d7221e11aa36eff71 // 

142 0x33baa46c4864899cddc865ae424818377aa50fbc 2023-09-26   0.004235000131375114   149293   0xeda8148ae04b03aa4aae94b27da7f3e8c3d644d8843757af3e600f7e6f781fa7 // 

144 0xfc03889fedfa5f9be5dca2cbb4568c246e1286a3 2023-09-26   0.003666008861485328   149293   0xeedc996eb55d96a7eb81627591099117c5f61f23570692b3548beaf387b7ac50 // 

145 0x6ac2599e86d96e57349fdf42cda6fa6ecaf9f799 2023-09-26   0.004073383446695009   149293   0x06031958c52f1e4b5c0c9620b35f37f126d1bb4dabd8432da8ea813522ffa3f7 // 

149 0x53184e7e1c797b515dbbd85a2b3886af8aaf7a8d 2023-09-26   0.003991201   149293   0xa016834a6cf6b384c8cd02b0632e03f568e8172397798cac3f4a6cb1a95cf711 // 

151 0x7b6d63c19fd5eb016e68740aca2af4d405be4d6a 2023-09-26   0.003389781878968284   149293   0x311bf292446e4ef8bd6391d54693aa630538bbf38a7b32ea7f5fe2267ad8e5ae // 

153 0x688d579b2546bcf0cc37c626fe2ed4f3193fdd94 2023-09-26   0.0034897075   149293   0xff86bc0eefcc9cc9d75857779b81c5fdc58b7fa37ed1a14f07199cbafe60988b // 

156 0x582fb3db01ae70fb5d3f3629c7da4fcbce44360b 2023-09-26   0.00434402134974809   149293   0x29cf23aa21dd7fb8419593b03e593c19d8c6a7ff9f96dbc1fcc2fd1b1dc70657 // 

158 0x6ea72a9cdd3e13c11c67c577a99bcfe33a66de01 2023-09-26   0.0038907055   149293   0x6cfce48d699b80fc52c73325803fc72570b8e4e70b548b9c7e9f4eb2037dc8b7 // 

159 0x55e9c3d3ca32c401d729e4afb66c30849df25211 2023-09-26   0.003691626   149293   0xa676fe20e70a458e0f330007ef3b776d5b0c77d9007b38f040422d683cd503b5 // 

160 0x66db22ea02216dd43a9b18855be3760e5ee8753a 2023-09-26   0.004390081   149293   0x84a54571168dd761e006bebfa59e7af9ed23787ae6e49f9ff5d460533fe209c1 // 

161 0xae804670d2a8d730395ac37153f7c28b13b89727 2023-09-26   0.004475106902862974   149293   0xd87ab17796a74594d5c1d45cf1b1e445067079fa3f3d5c70ffeb40d212ec40fd // 

162 0x4913f5e7505f4d2f5975eb7423d3f8b25b14e4c3 2023-09-26   0.004544607175062895   149293   0x01fd2b157905f2b453b4ceb9e435579917b86db1a5231261bec959dbc8bbe7c1 // 

163 0x897dee5919146c34ccbc8e70b6343bee5146a8f0 2023-09-26   0.004620612281158975   149293   0x5abfb5abda043ba92557bd0fef9d87e3300af75f88cc2fe4bb22179e1c6c14a1 // 

164 0xc4829240b8f52edc1b377547316a3466d163b9f0 2023-09-26   0.004452027169462872   149293   0xfa67aa0476025debf677370edc3ca1e2712b6e3ee36d958aa2d4758e5d175024 // 

165 0x60b05ce94531057d9adc95373c6c6774d8484592 2023-09-26   0.004654283386975974   149293   0x7b85fd1503b425e1b26acc6504508261bbfb961d5ad8a1bca690748f2dced491 // 

166 0x3289e5a2b17d855cbf5d83fd5fb77f451cba25e6 2023-09-26   0.0041902675   149293   0x156f834692083ef1570d9263b3e03a9b6b63a4ba545c9858f46a575a4389a1a7 // 

167 0x654a4fe5d575c2f1129832b67b27cb9547628729 2023-09-26   0.004388027   149293   0x6c70e62c4b9fb03b16dbce70e404615d890c91b18663a6eb5cc57749df4fb5f2 // 

168 0xe455e1f15926a5805875218af2a6ba3ecf1b6265 2023-09-26   0.002691626   149293   0x43650318599175e603e73cc312dfce722e325358a8ea050427c7fc149ce447ea // 

169 0xa2cd77f07762d8872b6c1c459b80f3ba95d338b3 2023-09-26   0.003351791228658284   149293   0x24d25e559a502b61427734bd37714eea7b551f0ae2cf13f68e1d4b06817d1da7 //

</details>



</details>
