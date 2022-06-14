
# PairFlash.sol
Title: Flash contract implementation
Notice: An example contract using the Uniswap V3 flash function

## Methods
```solidity
WETH9
```
Notice: An example contract using the Uniswap V3 flash function

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
factory
```
Notice: An example contract using the Uniswap V3 flash function

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
initFlash
```
Notice: An example contract using the Uniswap V3 flash function

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (address,address,uint24,uint256,uint256,uint24,uint24) | The parameters necessary for flash and the callback, passed in as FlashParams |


### Return Values
```solidity
refundETH
```
Notice: An example contract using the Uniswap V3 flash function

### Parameters

### Return Values
```solidity
swapRouter
```
Notice: An example contract using the Uniswap V3 flash function

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
sweepToken
```
Notice: An example contract using the Uniswap V3 flash function

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The contract address of the token which will be transferred to `recipient` |
| amountMinimum | uint256 | The minimum amount of token required for a transfer |
| recipient | address | The destination address of the token |


### Return Values
```solidity
uniswapV3FlashCallback
```
Notice: An example contract using the Uniswap V3 flash function

### Parameters
| Name | Type | Description |
|---|---|---|
| fee0 | uint256 | The fee from calling flash for token0 |
| fee1 | uint256 | The fee from calling flash for token1 |
| data | bytes | The data needed in the callback passed as FlashCallbackData from `initFlash` |


### Return Values
```solidity
unwrapWETH9
```
Notice: An example contract using the Uniswap V3 flash function

### Parameters
| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | The minimum amount of WETH9 to unwrap |
| recipient | address | The address receiving ETH |


### Return Values

### Events

### Errors

