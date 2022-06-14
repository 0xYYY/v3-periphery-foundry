
# ISwapRouter.sol
Title: Router token swapping functionality
Notice: Functions for swapping tokens via Uniswap V3

## Methods
```solidity
exactInput
```
Notice: Functions for swapping tokens via Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (bytes,address,uint256,uint256,uint256) | The parameters necessary for the multi-hop swap, encoded as `ExactInputParams` in calldata |


### Return Values
| Name | Type | Description |
|---|---|---|
| amountOut | uint256 | The amount of the received token |

```solidity
exactInputSingle
```
Notice: Functions for swapping tokens via Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (address,address,uint24,address,uint256,uint256,uint256,uint160) | The parameters necessary for the swap, encoded as `ExactInputSingleParams` in calldata |


### Return Values
| Name | Type | Description |
|---|---|---|
| amountOut | uint256 | The amount of the received token |

```solidity
exactOutput
```
Notice: Functions for swapping tokens via Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (bytes,address,uint256,uint256,uint256) | The parameters necessary for the multi-hop swap, encoded as `ExactOutputParams` in calldata |


### Return Values
| Name | Type | Description |
|---|---|---|
| amountIn | uint256 | The amount of the input token |

```solidity
exactOutputSingle
```
Notice: Functions for swapping tokens via Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (address,address,uint24,address,uint256,uint256,uint256,uint160) | The parameters necessary for the swap, encoded as `ExactOutputSingleParams` in calldata |


### Return Values
| Name | Type | Description |
|---|---|---|
| amountIn | uint256 | The amount of the input token |

```solidity
uniswapV3SwapCallback
```
Notice: Functions for swapping tokens via Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| amount0Delta | int256 | The amount of token0 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token0 to the pool. |
| amount1Delta | int256 | The amount of token1 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token1 to the pool. |
| data | bytes | Any data passed through by the caller via the IUniswapV3PoolActions#swap call |


### Return Values

### Events

### Errors

