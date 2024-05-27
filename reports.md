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
The first 21 addresses within the cluster are linked to the same OKX deposit address: 0x151c6d618AF9305CCa87Dac37578dDC9AAbD9382. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.

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
The first 21 addresses within the cluster are linked to the same OKX deposit address: 0x151c6d618AF9305CCa87Dac37578dDC9AAbD9382. The remaining addresses are interconnected with numerous addresses within the cluster, often multiple times.



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
