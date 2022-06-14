
# PeripheryPaymentsWithFee.sol

## Methods
```solidity
WETH9
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
factory
```

### Parameters

### Return Values
| Name | Type | Description |
|---|---|---|
|  | address |  |

```solidity
refundETH
```

### Parameters

### Return Values
```solidity
sweepToken
```

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
unwrapWETH9
```

### Parameters
| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | The minimum amount of WETH9 to unwrap |
| recipient | address | The address receiving ETH |


### Return Values
```solidity
unwrapWETH9WithFee
```

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

