# 清算

## 清算例子

假设当您在 Bend DAO 中抵押 BAYC 即时借款 40 ETH 时，BAYC 地板价是 100 ETH。

如果地板价跌至 44 ETH，由于您的 NFT 支持的借贷的健康系数低于 1，48 小时清算保护将被触发。

健康系数 = (44 \* 90%) / (40 + 利息) < 1&#x20;

健康系数 = (地板价 \* 清算阈值) / 含息债务。

## 什么是健康系数？

健康系数是您存入的 NFT 对借出的 ETH 及其基础价值的安全性的数字表示。该值越高，说明您的资金状况在清算情况下越安全。

如果健康系数达到 1，将触发对您抵押品的清算。健康系数低于 1 的抵押品将会被清算。对于健康系数 = 2，抵押品价值相比于借款会减少二分之一 ——— 即 50%。

健康系数取决于您的抵押品相比于您借出资金的价值的清算阈值。

您可以在[风险参数](../risk/nft-risk-parameters.md)部分找到所有抵押品的参数。

## 当我的健康系数降低时会发生什么？

健康系数取决于您抵押资产价值的波动将上升或下降。如果您的健康指数上升，您的借款状况将会改善，使清算阈值变得更加不可能达到。若您的抵押资产相较借出资产的价值下降，健康系数将下降，导致清算的风险增加。

## **Bend 是如何计算抵押的 NFT 的价值的？**

当前 NFT 地板价被用作抵押 NFT 的价格推送。\*\*\*\* 原始价格数据来自最知名的NFT市场 —— OpenSea。Bend 上的抵押品价值以以太坊计价，而非 USDT。

## **有无计划升级 NFT 的价格推送设计？**

由于现在市场上没有成熟的 NFT 价格推送解决方案，使用地板价可能是最安全的选择。当出现更好的选择时，Bend 会考虑使用新的 NFT 预言机。

## **为什么 Bend 上面不会发生市场清算危机？**


48 小时的清算保护和 NFT 拍卖机制的存在意味着 NFT 不会被立即清算。同时，清算人的出价必须等同于 OpenSea 的地板价。

更多关于[ 48h 清算保护](../highlights/48h-liquidation-protection.md)的细节。

## **当清算发生时会怎么样？**

当清算发生时，智能合约会触发一个 48 小时的清算保护机制。借款人（拥有抵押的 NFT 的用户）将能够在 48 小时的时间窗口内偿还贷款。\
\
Bend 会设置一个 Discord 机器人更新借款人的借贷情况。\
\
在 48 小时的清算保护期内，Bend 将启动 NFT 拍卖。

## **Bend 上的清算阈值是什么？**

如果抵押品的清算阈值为 90%，当债务价值为抵押品价值的 80% 时，贷款将被清算。每种抵押品有专门规定的清算阈值，并以百分点表示。

## **如果以太坊的价格下跌，我的贷款是否会被清算？**

所有 NFT 在 Bend 上都以以太坊计价而非 USDT。以太坊价格和 NFT 的价格没有必然联系。

## **Does the borrower need to keep paying interest while the 48-hour liquidation protection mechanism is active?**

Yes. Because the NFT-backed loan is still active during the 48-hour liquidation protection. For safety and fairness, borrowers need to pay a penalty (1% of the bid price in default) to the liquidator, even after NFT floor prices recover to the normal price.

## **What if no liquidator shows up?**

We do not anticipate this happening frequently, if ever. However, in the case it theoretically would, for the safety of the protocol, the Bend DAO will participate in the NFT auction if no third-party liquidator is interested in the collateralized bluechip NFT. Security is always the first priority with Bend.

## What if the floor price drops, the auction bid can’t cover it?

It will not happen, since the bid must be 1) more than 95% of the floor price; 2) bigger than the total accumulated debt; 3) higher than the previous bid.

If no liquidator shows up, for the safety of the protocol, the Bend DAO will participate in the NFT auction if no third-party liquidator is interested in the collateralized bluechip NFT. Security is always the first priority with Bend.

## What will happen if floor price drop to 0?

Bluechip NFTs are fast-growing assets that appreciate faster than ETH and the whole market is still early.

Bend will only lists high quality bluechip NFTs that have been recognized by the market, and they have at least experienced multiple cycles of ups and downs.

Bend is continuously monitoring the market indicators of bluechip NFTs, and timely adjusts risk parameters through community governance, such as collateral ratio and delisting NFTs.

