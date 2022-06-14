
# IQuoterV2.sol
Title: QuoterV2 Interface
Details: These functions are not marked view because they rely on calling non-view functions and reverting to compute the result. They are also not gas efficient and should not be called on-chain.
Notice: Supports quoting the calculated amounts from exact input or exact output swaps.For each pool also tells you the number of initialized ticks crossed and the sqrt price of the pool after the swap.

## Methods
```solidity
quoteExactInput
```
Details: These functions are not marked view because they rely on calling non-view functions and reverting to compute the result. They are also not gas efficient and should not be called on-chain.
Notice: Supports quoting the calculated amounts from exact input or exact output swaps.For each pool also tells you the number of initialized ticks crossed and the sqrt price of the pool after the swap.

### Parameters
| Name | Type | Description |
|---|---|---|
| path | bytes | The path of the swap, i.e. each token pair and the pool fee |
| amountIn | uint256 | The amount of the first token to swap |


### Return Values
| Name | Type | Description |
|---|---|---|
| amountOut | uint256 | The amount of the last token that would be received |
| sqrtPriceX96AfterList | uint160[] | List of the sqrt price after the swap for each pool in the path |
| initializedTicksCrossedList | uint32[] | List of the initialized ticks that the swap crossed for each pool in the path |
| gasEstimate | uint256 | The estimate of the gas that the swap consumes |

```solidity
quoteExactInputSingle
```
Details: These functions are not marked view because they rely on calling non-view functions and reverting to compute the result. They are also not gas efficient and should not be called on-chain.
Notice: Supports quoting the calculated amounts from exact input or exact output swaps.For each pool also tells you the number of initialized ticks crossed and the sqrt price of the pool after the swap.

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (address,address,uint256,uint24,uint160) | The params for the quote, encoded as `QuoteExactInputSingleParams` tokenIn The token being swapped in tokenOut The token being swapped out fee The fee of the token pool to consider for the pair amountIn The desired input amount sqrtPriceLimitX96 The price limit of the pool that cannot be exceeded by the swap |


### Return Values
| Name | Type | Description |
|---|---|---|
| amountOut | uint256 | The amount of `tokenOut` that would be received |
| sqrtPriceX96After | uint160 | The sqrt price of the pool after the swap |
| initializedTicksCrossed | uint32 | The number of initialized ticks that the swap crossed |
| gasEstimate | uint256 | The estimate of the gas that the swap consumes |

```solidity
quoteExactOutput
```
Details: These functions are not marked view because they rely on calling non-view functions and reverting to compute the result. They are also not gas efficient and should not be called on-chain.
Notice: Supports quoting the calculated amounts from exact input or exact output swaps.For each pool also tells you the number of initialized ticks crossed and the sqrt price of the pool after the swap.

### Parameters
| Name | Type | Description |
|---|---|---|
| path | bytes | The path of the swap, i.e. each token pair and the pool fee. Path must be provided in reverse order |
| amountOut | uint256 | The amount of the last token to receive |


### Return Values
| Name | Type | Description |
|---|---|---|
| amountIn | uint256 | The amount of first token required to be paid |
| sqrtPriceX96AfterList | uint160[] | List of the sqrt price after the swap for each pool in the path |
| initializedTicksCrossedList | uint32[] | List of the initialized ticks that the swap crossed for each pool in the path |
| gasEstimate | uint256 | The estimate of the gas that the swap consumes |

```solidity
quoteExactOutputSingle
```
Details: These functions are not marked view because they rely on calling non-view functions and reverting to compute the result. They are also not gas efficient and should not be called on-chain.
Notice: Supports quoting the calculated amounts from exact input or exact output swaps.For each pool also tells you the number of initialized ticks crossed and the sqrt price of the pool after the swap.

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (address,address,uint256,uint24,uint160) | The params for the quote, encoded as `QuoteExactOutputSingleParams` tokenIn The token being swapped in tokenOut The token being swapped out fee The fee of the token pool to consider for the pair amountOut The desired output amount sqrtPriceLimitX96 The price limit of the pool that cannot be exceeded by the swap |


### Return Values
| Name | Type | Description |
|---|---|---|
| amountIn | uint256 | The amount required as the input for the swap in order to receive `amountOut` |
| sqrtPriceX96After | uint160 | The sqrt price of the pool after the swap |
| initializedTicksCrossed | uint32 | The number of initialized ticks that the swap crossed |
| gasEstimate | uint256 | The estimate of the gas that the swap consumes |


### Events

### Errors

