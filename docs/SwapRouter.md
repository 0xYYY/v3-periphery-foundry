
# SwapRouter.sol
Title: Uniswap V3 Swap Router
Notice: Router for stateless execution of swaps against Uniswap V3

## Methods
```solidity
WETH9
```
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
exactInput
```
Notice: Router for stateless execution of swaps against Uniswap V3

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
Notice: Router for stateless execution of swaps against Uniswap V3

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
Notice: Router for stateless execution of swaps against Uniswap V3

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
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| params | (address,address,uint24,address,uint256,uint256,uint256,uint160) | The parameters necessary for the swap, encoded as `ExactOutputSingleParams` in calldata |


### Return Values
| Name | Type | Description |
|---|---|---|
| amountIn | uint256 | The amount of the input token |

```solidity
factory
```
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
multicall
```
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| data | bytes[] | The encoded function data for each of the calls to make to this contract |


### Return Values
| Name | Type | Description |
|---|---|---|
| results | bytes[] | The results from each of the calls passed in via data |

```solidity
refundETH
```
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters

### Return Values
```solidity
selfPermit
```
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| value | uint256 | The amount that can be spent of token |
| deadline | uint256 | A timestamp, the current blocktime must be less than or equal to this timestamp |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values
```solidity
selfPermitAllowed
```
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| nonce | uint256 | The current nonce of the owner |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values
```solidity
selfPermitAllowedIfNecessary
```
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| nonce | uint256 | The current nonce of the owner |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values
```solidity
selfPermitIfNecessary
```
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| value | uint256 | The amount that can be spent of token |
| deadline | uint256 | A timestamp, the current blocktime must be less than or equal to this timestamp |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values
```solidity
sweepToken
```
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The contract address of the token which will be transferred to `recipient` |
| amountMinimum | uint256 | The minimum amount of token required for a transfer |
| recipient | address | The destination address of the token |


### Return Values
```solidity
sweepTokenWithFee
```
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address |  |
| amountMinimum | uint256 |  |
| recipient | address |  |
| feeBips | uint256 |  |
| feeRecipient | address |  |


### Return Values
```solidity
uniswapV3SwapCallback
```
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| amount0Delta | int256 | The amount of token0 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token0 to the pool. |
| amount1Delta | int256 | The amount of token1 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token1 to the pool. |
| _data | bytes |  |


### Return Values
```solidity
unwrapWETH9
```
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | The minimum amount of WETH9 to unwrap |
| recipient | address | The address receiving ETH |


### Return Values
```solidity
unwrapWETH9WithFee
```
Notice: Router for stateless execution of swaps against Uniswap V3

### Parameters
| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 |  |
| recipient | address |  |
| feeBips | uint256 |  |
| feeRecipient | address |  |


### Return Values

### Events

### Errors

