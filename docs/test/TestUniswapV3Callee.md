
# TestUniswapV3Callee.sol

## Methods
```solidity
swap0ForExact1
```

### Parameters
| Name | Type | Description |
|---|---|---|
| pool | address |  |
| amount1Out | uint256 |  |
| recipient | address |  |
| sqrtPriceLimitX96 | uint160 |  |


### Return Values
```solidity
swap1ForExact0
```

### Parameters
| Name | Type | Description |
|---|---|---|
| pool | address |  |
| amount0Out | uint256 |  |
| recipient | address |  |
| sqrtPriceLimitX96 | uint160 |  |


### Return Values
```solidity
swapExact0For1
```

### Parameters
| Name | Type | Description |
|---|---|---|
| pool | address |  |
| amount0In | uint256 |  |
| recipient | address |  |
| sqrtPriceLimitX96 | uint160 |  |


### Return Values
```solidity
swapExact1For0
```

### Parameters
| Name | Type | Description |
|---|---|---|
| pool | address |  |
| amount1In | uint256 |  |
| recipient | address |  |
| sqrtPriceLimitX96 | uint160 |  |


### Return Values
```solidity
uniswapV3SwapCallback
```

### Parameters
| Name | Type | Description |
|---|---|---|
| amount0Delta | int256 | The amount of token0 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token0 to the pool. |
| amount1Delta | int256 | The amount of token1 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token1 to the pool. |
| data | bytes | Any data passed through by the caller via the IUniswapV3PoolActions#swap call |


### Return Values

### Events

### Errors

