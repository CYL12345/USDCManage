# USDCManage
Build an application that enables multichain USDC payments and payouts, remittances, treasury rebalancing, swaps, or seamless USDC purchases.

```mermaid
graph TD;
   用户界面-->API网关
   API网关-->支付模块
   API网关-->跨链路由
   API网关-->资金管理
   支付模块-->EVM链
   支付模块-->SOL链
   支付模块-->其他链
   跨链路由-->跨链桥接协议
   跨链桥接协议-->Connext
   跨链桥接协议-->Wormhole
   资金管理-->自平衡引擎
