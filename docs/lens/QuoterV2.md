
# QuoterV2.sol

    
Provides quotes for swaps
These functions are not gas efficient and should _not_ be called on chain. Instead, optimistically execute the swap and check the amounts in the callback.

    
*Allows getting the expected amount out or amount in for a given swap without executing the swap*
## Methods
### WETH9
```solidity
WETH9() external view returns (address)
```

            
These functions are not gas efficient and should _not_ be called on chain. Instead, optimistically execute the swap and check the amounts in the callback.

            
*Allows getting the expected amount out or amount in for a given swap without executing the swap*
#### Return Values

| Name | Type | Description |
|---|---|---|
|  | address | - |

### factory
```solidity
factory() external view returns (address)
```

            
These functions are not gas efficient and should _not_ be called on chain. Instead, optimistically execute the swap and check the amounts in the callback.

            
*Allows getting the expected amount out or amount in for a given swap without executing the swap*
#### Return Values

| Name | Type | Description |
|---|---|---|
|  | address | - |

### quoteExactInput
```solidity
quoteExactInput(bytes path, uint256 amountIn) external nonpayable returns (uint256 amountOut, uint160[] sqrtPriceX96AfterList, uint32[] initializedTicksCrossedList, uint256 gasEstimate)
```

            
These functions are not gas efficient and should _not_ be called on chain. Instead, optimistically execute the swap and check the amounts in the callback.

            
*Allows getting the expected amount out or amount in for a given swap without executing the swap*
#### Parameters

| Name | Type | Description |
|---|---|---|
| path | bytes | The path of the swap, i.e. each token pair and the pool fee |
| amountIn | uint256 | The amount of the first token to swap |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amountOut | uint256 | The amount of the last token that would be received |
| sqrtPriceX96AfterList | uint160[] | List of the sqrt price after the swap for each pool in the path |
| initializedTicksCrossedList | uint32[] | List of the initialized ticks that the swap crossed for each pool in the path |
| gasEstimate | uint256 | The estimate of the gas that the swap consumes |

### quoteExactInputSingle
```solidity
quoteExactInputSingle((address,address,uint256,uint24,uint160) params) external nonpayable returns (uint256 amountOut, uint160 sqrtPriceX96After, uint32 initializedTicksCrossed, uint256 gasEstimate)
```

            
These functions are not gas efficient and should _not_ be called on chain. Instead, optimistically execute the swap and check the amounts in the callback.

            
*Allows getting the expected amount out or amount in for a given swap without executing the swap*
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (address,address,uint256,uint24,uint160) | The params for the quote, encoded as `QuoteExactInputSingleParams` tokenIn The token being swapped in tokenOut The token being swapped out fee The fee of the token pool to consider for the pair amountIn The desired input amount sqrtPriceLimitX96 The price limit of the pool that cannot be exceeded by the swap |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amountOut | uint256 | The amount of `tokenOut` that would be received |
| sqrtPriceX96After | uint160 | The sqrt price of the pool after the swap |
| initializedTicksCrossed | uint32 | The number of initialized ticks that the swap crossed |
| gasEstimate | uint256 | The estimate of the gas that the swap consumes |

### quoteExactOutput
```solidity
quoteExactOutput(bytes path, uint256 amountOut) external nonpayable returns (uint256 amountIn, uint160[] sqrtPriceX96AfterList, uint32[] initializedTicksCrossedList, uint256 gasEstimate)
```

            
These functions are not gas efficient and should _not_ be called on chain. Instead, optimistically execute the swap and check the amounts in the callback.

            
*Allows getting the expected amount out or amount in for a given swap without executing the swap*
#### Parameters

| Name | Type | Description |
|---|---|---|
| path | bytes | The path of the swap, i.e. each token pair and the pool fee. Path must be provided in reverse order |
| amountOut | uint256 | The amount of the last token to receive |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amountIn | uint256 | The amount of first token required to be paid |
| sqrtPriceX96AfterList | uint160[] | List of the sqrt price after the swap for each pool in the path |
| initializedTicksCrossedList | uint32[] | List of the initialized ticks that the swap crossed for each pool in the path |
| gasEstimate | uint256 | The estimate of the gas that the swap consumes |

### quoteExactOutputSingle
```solidity
quoteExactOutputSingle((address,address,uint256,uint24,uint160) params) external nonpayable returns (uint256 amountIn, uint160 sqrtPriceX96After, uint32 initializedTicksCrossed, uint256 gasEstimate)
```

            
These functions are not gas efficient and should _not_ be called on chain. Instead, optimistically execute the swap and check the amounts in the callback.

            
*Allows getting the expected amount out or amount in for a given swap without executing the swap*
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (address,address,uint256,uint24,uint160) | The params for the quote, encoded as `QuoteExactOutputSingleParams` tokenIn The token being swapped in tokenOut The token being swapped out fee The fee of the token pool to consider for the pair amountOut The desired output amount sqrtPriceLimitX96 The price limit of the pool that cannot be exceeded by the swap |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amountIn | uint256 | The amount required as the input for the swap in order to receive `amountOut` |
| sqrtPriceX96After | uint160 | The sqrt price of the pool after the swap |
| initializedTicksCrossed | uint32 | The number of initialized ticks that the swap crossed |
| gasEstimate | uint256 | The estimate of the gas that the swap consumes |

### uniswapV3SwapCallback
```solidity
uniswapV3SwapCallback(int256 amount0Delta, int256 amount1Delta, bytes path) external view
```

            
These functions are not gas efficient and should _not_ be called on chain. Instead, optimistically execute the swap and check the amounts in the callback.

            
*Allows getting the expected amount out or amount in for a given swap without executing the swap*
#### Parameters

| Name | Type | Description |
|---|---|---|
| amount0Delta | int256 | The amount of token0 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token0 to the pool. |
| amount1Delta | int256 | The amount of token1 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token1 to the pool. |
| path | bytes | - |


