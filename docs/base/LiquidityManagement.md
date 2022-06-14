
# LiquidityManagement.sol
Title: Liquidity management functions
Notice: Internal functions for safely managing liquidity in Uniswap V3

## Methods
```solidity
WETH9
```
Notice: Internal functions for safely managing liquidity in Uniswap V3

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
factory
```
Notice: Internal functions for safely managing liquidity in Uniswap V3

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
refundETH
```
Notice: Internal functions for safely managing liquidity in Uniswap V3

### Parameters

### Return Values
```solidity
sweepToken
```
Notice: Internal functions for safely managing liquidity in Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The contract address of the token which will be transferred to `recipient` |
| amountMinimum | uint256 | The minimum amount of token required for a transfer |
| recipient | address | The destination address of the token |


### Return Values
```solidity
uniswapV3MintCallback
```
Notice: Internal functions for safely managing liquidity in Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| amount0Owed | uint256 | The amount of token0 due to the pool for the minted liquidity |
| amount1Owed | uint256 | The amount of token1 due to the pool for the minted liquidity |
| data | bytes | Any data passed through by the caller via the IUniswapV3PoolActions#mint call |


### Return Values
```solidity
unwrapWETH9
```
Notice: Internal functions for safely managing liquidity in Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | The minimum amount of WETH9 to unwrap |
| recipient | address | The address receiving ETH |


### Return Values

### Events

### Errors

