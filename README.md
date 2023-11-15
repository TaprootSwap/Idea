# Idea
Ordinal inscriptions make trading visible and verifiable on-chain.

Since there are no smart contracts on the BTC mainnet network, it is impossible to store assets through smart contracts. However, from another perspective, a large number of smart contracts are now upgradeable, and smart contract creators can transfer the deposited assets by upgrading the smart contracts, even if the smart contracts can pass the code audit smoothly. Therefore, it is not safe to store assets through smart contracts.

On the other hand, there are still a large number of deposit users on CEXs, and the biggest problem that people criticize CEXs for is that their trading data is a black box, which leads to the possibility of CEXs making profits from fake transactions (that is, selling assets that they should not have at will, and then buying back the assets at a low price to achieve asset balance).

Therefore, we conceived a trading method that uses the tamper-proof feature of Ordinals: recording transaction records on-chain by Ordinal Inscriptions, and completing transactions off-chain according to the content broadcast by Ordinal Inscriptions, making the entire trading visible and verifiable on-chain.

BRC-20-lp & BRC-20-swap

Based on this idea, we experimented with whether we could use the AMM model to build a P2Pool trading protocol for BRC-20. This protocol consists of two main parts:

Creating liquidity pools and recording adding/withdrawing liquidity

Recording user behavior when swapping assets with liquidity pools

Therefore, we created two protocols: Liquidity Provider Protocol—BRC-20-lp, and Tokens Swap Protocol—BRC-20-swap.
