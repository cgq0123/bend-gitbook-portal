# Flash Claim FAQ

## Q: 当我的 NFT 存入 Bend 时，我如何能领取我的空投？&#x20;

A: Flash Claim 功能就是为这种情况设计的。在网页面板上找到 “Flash Claim”，借款人可以领取相关空投。 [https://www.benddao.xyz/app/flash-claim](https://www.benddao.xyz/app/flash-claim)

## Q: Bend 如何知道我是否有资格获得空投？&#x20;

A: 如果您持有相关的 boundNFT，您可以领取空投。所有借款人在 Bend 成功存入 NFT 时都会收到 boundNFT。

## Q: Flash Claim 将支持哪种空投方式？&#x20;

A: Flash Claim 支持两种空投方式：1）项目直接空投到持有者地址；2）空投需要持有人领取。更多细节见：https://docs.benddao.xyz/portal/user-guides/flashclaim

## Q: 如果项目直接空投到持有人的地址，Bend 怎么能知道哪个空投的代币属于哪个借款人？&#x20;

A: Bend DAO 遵循项目设定的空投规则。可以支持特定空投和随机空投。

## Q: 如果是随机空投，Bend DAO 是如何分配空投的？&#x20;

A: Bend 上的分配过程也是随机的。为了公平和安全，Bend 的随机算法是基于 [Chainlink VRF 架构](https://vrf.chain.link/mainnet) 来分发代币。&#x20;

Chainlink 上的 VRF 的订阅 id：[81](https://vrf.chain.link/mainnet/81)。

空投代币分配的代码在[ ](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropDistribution.sol)Github: [AirdropDistribution.sol](https://github.com/BoundNFT/boundnft-protocol/blob/main/contracts/misc/AirdropDistribution.sol).&#x20;

合约代码在[ ](https://etherscan.io/address/0x6D187449A5664DD87E58A9d3b982989AaeA469BD)Etherscan: [0x6D187449A5664DD87E58A9d3b982989AaeA469BD](https://etherscan.io/address/0x6D187449A5664DD87E58A9d3b982989AaeA469BD).

## Q: 如果我错过了领取期怎么办？&#x20;

A: 您永远可以在 Bend 上面 Flash Claim 您的空投。您的空投永不过期。

## Q: Can I Flash Claim if I have no knowledge of programming?&#x20;

A: You can simply click the Flash Claim button to claim your airdrops. There are no programming requirements.

## Q: What is boundNFT?&#x20;

A: For NFT-backed loans, when the borrower deposits an NFT in Bend DAO, a boundNFT will be minted as a Debt NFT. For Custody, when the NFT holder deposits an NFT in Bend DAO, a boundNFT will be minted as a receipt NFT.&#x20;

More details of boundNFT https://docs.benddao.xyz/portal/highlights/true-ownership

## Q: Is the Flash Claim open-sourced?&#x20;

A: Yes. Visit BoundNFT Github to find more details. https://github.com/BoundNFT/boundnft-protocol/tree/main/contracts

## Q: Can I realize the Flash Claim by myself if I have programming experience?&#x20;

A: Yes. Users also can write a contract to implement the Flash Claim. Please check the demo on Github. https://github.com/BendDAO/bend-flashclaim-demo

## Q: What kind of airdrops will be supported on Bend?&#x20;

A: Yuga Metaverse Land, of course. Technically, all airdrops that are related to the collaterals can be supported. Bend supported collaterals are BAYC, CryptoPunks, MAYC, Azuki, CloneX, and Doodles.

Feel free to find the team in Discord if you want us to support other great airdrops.
