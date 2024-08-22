---
head:
  - - meta
    - property: og:title
      content: LP Positions
  - - meta
    - name: description
      content: Learn how to provide liquidity on BEX, including minting and managing LP positions, and understanding the concept of impermanent loss.
  - - meta
    - property: og:description
      content: Learn how to provide liquidity on BEX, including minting and managing LP positions, and understanding the concept of impermanent loss.
---

# Liquidity Provision

Users can provide liquidity to BEX by committing tokens to a specific pool. _Liquidity providers_ (LPs) earn a yield on their capital generated by the swap fees paid into the pool. In return for these fees and other potential benefits, LPs must deal with the fact that the collateral they deposit is not fixed. LP positions continuously rebalance between the two tokens in the pair as swaps occur in the pool.

This rebalancing can impose a cost on LPs in the form of _impermanent loss_ (IL), which is the difference between the value of the rebalanced position and an equivalent static portfolio of the two assets. The larger the price ratio of the assets in the pool moves from when the user first deposited, the larger the IL cost experienced by the LP.

LPs on BEX provide full-range liquidity, meaning that users' liquidity is always active at every possible price point in the pool.

Users can provide BEX liquidity and review available options on bArtio here: https://bartio.bex.berachain.com/pools

![BEX pools](/assets/bex-pools.png)

### Adding Liquidity

_Adding Liquidity_ is the process of providing the two constituent tokens of a liquidity pool to either 1) create a new LP position, or 2) commit additional capital to a pre-existing LP position.

![Adding Liquidity](/assets/adding-liquidity.png)

When adding liquidity to an LP position, users have the following parameters to choose from:

- The token pair to provide liquidity for
- Deposit quantity, which can be fixed in terms of either side of the pair
- Maximum slippage and transaction deadline

### Managing LP Positions

Users can view their existing LP positions through the BEX web app.

To remove liquidity from a specific position, users can _burn_ their LP tokens. This removes the liquidity from the pool and returns the underlying collateral (based on the current token prices) to the user.