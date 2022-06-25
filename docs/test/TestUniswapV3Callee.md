
# TestUniswapV3Callee.sol

    

    
## Methods
### swap0ForExact1
```solidity
swap0ForExact1(address pool, uint256 amount1Out, address recipient, uint160 sqrtPriceLimitX96) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | - |
| amount1Out | uint256 | - |
| recipient | address | - |
| sqrtPriceLimitX96 | uint160 | - |

### swap1ForExact0
```solidity
swap1ForExact0(address pool, uint256 amount0Out, address recipient, uint160 sqrtPriceLimitX96) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | - |
| amount0Out | uint256 | - |
| recipient | address | - |
| sqrtPriceLimitX96 | uint160 | - |

### swapExact0For1
```solidity
swapExact0For1(address pool, uint256 amount0In, address recipient, uint160 sqrtPriceLimitX96) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | - |
| amount0In | uint256 | - |
| recipient | address | - |
| sqrtPriceLimitX96 | uint160 | - |

### swapExact1For0
```solidity
swapExact1For0(address pool, uint256 amount1In, address recipient, uint160 sqrtPriceLimitX96) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| pool | address | - |
| amount1In | uint256 | - |
| recipient | address | - |
| sqrtPriceLimitX96 | uint160 | - |

### uniswapV3SwapCallback
```solidity
uniswapV3SwapCallback(int256 amount0Delta, int256 amount1Delta, bytes data) external nonpayable
```

            
In the implementation you must pay the pool tokens owed for the swap. The caller of this method must be checked to be a UniswapV3Pool deployed by the canonical UniswapV3Factory. amount0Delta and amount1Delta can both be 0 if no tokens were swapped.

            
*Called to `msg.sender` after executing a swap via IUniswapV3Pool#swap.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| amount0Delta | int256 | The amount of token0 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token0 to the pool. |
| amount1Delta | int256 | The amount of token1 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token1 to the pool. |
| data | bytes | Any data passed through by the caller via the IUniswapV3PoolActions#swap call |


