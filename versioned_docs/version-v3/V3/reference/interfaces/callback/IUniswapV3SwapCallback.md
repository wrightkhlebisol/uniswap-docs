Any contract that calls IUniswapV3PoolActions#swap must implement this interface


## Functions
### uniswapV3SwapCallback
```solidity
  function uniswapV3SwapCallback(
    int256 amount0Delta, int256 amount1Delta, bytes data
  ) external
```
Called on `msg.sender` after performing a swap and transferring any output tokens to the recipient

The caller of this method must be checked to be a UniswapV3Pool deployed by the canonical factory.
Both amount0 and amount1 can be 0.

#### Parameters:
| Name | Type | Description                                                          |
| :--- | :--- | :------------------------------------------------------------------- |
|`amount0Delta` | int256 | The amount of token0 that was sent (negative) or must be received (positive) by the pool by
the end of the swap. If positive, the callback must send that amount of token0 to the pool.
|`amount1Delta` | int256 | The amount of token1 that was sent (negative) or must be received (positive) by the pool by
the end of the swap. If positive, the callback must send that amount of token1 to the pool.
|`data` | bytes | Any data passed through by the caller via the IUniswapV3PoolActions#swap call

