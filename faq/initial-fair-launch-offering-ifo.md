# 首次公平发售（IFO）

## Q: 为什么叫 IFO？

A: F 代表 Fair Launch（即公平启动）。

* 无 VC（风险投资资金）；
* 无 预售；
* 无 白名单；
* 持币人获得 **100%** 收益。

## Q: 什么是 BEND IFO？

A: 首次公平发售（IFO）是 BEND 代币[公平启动](../highlights/fair-launch.md)的一部分。BEND IFO 是一种从公众中汇集 ETH 的募资方式。


**66%** 募集的 ETH 的将会用于 Bend 的 ETH 借贷池，**34%** 的 ETH 将用于 Bend 的开发运营。

规则如下：

* 1,000,000,000（10%）的 BEND 代币将被分配给首次公平发售（IFO）；
* 向公众开放；
* 每个参与者的 ETH 配额没有限制；
* 1 ETH = 333,333 BEND；
* IFO 之后，所有未售出的 BEND 将被纳入 DAO 金库；
* 每个参与者都可以选择 IFO 期间的锁定期，从 0 周到 4 年。
* 从锁定的那一刻起，持有人将分享协议收入。

## Q: 我能用 BEND 代币做什么？

A: BEND 持有人可以质押 BEND 获得 BEND 选票（即 veBEND）。

如果您参与 IFO，您的 BEND 将被自动质押。您将获得 veBEND 代币。您锁定 BEND 代币的时间越长，您获得的 veBEND 越多。

**veBEND** 有两个主要用途：**投票**以及**收益分成**。

**投票**

veBEND 持有者可以参与投票，决定 Bend 协议可以支持哪些 NFT 作为抵押品以借出 ETH 并提供流动性。只要支持的 NFT 的流动性得到改善，所有 NFT 持有者都会受益。

在主网启动之前，veBEND 持有人将投票选出 7 个蓝筹 NFT 中的 4 个，它们将获得初始 ETH 借贷池的支持。7 个 NFT 系列是 **Mutant Ape YC, Cool Cats, Doodles, CLONE X, Azuki, World of Women** 和 **CyberKongz**。

**收益分成**

协议收入的 100% 将被分配给质押 BEND 的 veBEND 持有者。

## Q: 谁可以参与 IFO？

A: 所有在以太主网拥有去中心化钱包的人都可以参与。无白名单，无 KYC。

## Q: 我可以购买多少 BEND？

A: 每个参与者没有 ETH 配额限制。比率为 1 ETH = 333,333 BEND。

## Q: 是否有任何强制锁仓？

A: 无。

## Q: 如果我参与了 IFO，我能得到什么？

BEND 选票。veBEND 就是质押中的 BEND。当您把 veBEND 代币地址添加到您的钱包里时，您就可以看到您的 veBEND 余额。

veBEND 是 BEND 选票（vote-escrowed BEND）的缩写，也就是您在质押 BEND 时获得的代币。您质押 BEND 的时间越长，您获得的 veBEND 就越多。

## Q: 那么我将会获得多少 veBEND 代币呢？

A: 最高锁定期为四年时间。公式概述如下：

MAXTIME = 4 \* 365 \* 86400\
unlock\_time < (block\_time + MAXTIME) veBEND\_amount = BEND\_locked\_amount / MAXTIME \* (unlock\_time - block\_time)
