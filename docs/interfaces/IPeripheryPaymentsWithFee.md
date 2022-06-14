
# IPeripheryPaymentsWithFee.sol
Title: Periphery Payments
Notice: Functions to ease deposits and withdrawals of ETH

## Methods
### refundETH
```solidity
refundETH() external payable
```
Notice: Functions to ease deposits and withdrawals of ETH
### sweepToken
```solidity
sweepToken(address token, uint256 amountMinimum, address recipient) external payable
```
Notice: Functions to ease deposits and withdrawals of ETH
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The contract address of the token which will be transferred to `recipient` |
| amountMinimum | uint256 | The minimum amount of token required for a transfer |
| recipient | address | The destination address of the token |

### sweepTokenWithFee
```solidity
sweepTokenWithFee(address token, uint256 amountMinimum, address recipient, uint256 feeBips, address feeRecipient) external payable
```
Notice: Functions to ease deposits and withdrawals of ETH
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | - |
| amountMinimum | uint256 | - |
| recipient | address | - |
| feeBips | uint256 | - |
| feeRecipient | address | - |

### unwrapWETH9
```solidity
unwrapWETH9(uint256 amountMinimum, address recipient) external payable
```
Notice: Functions to ease deposits and withdrawals of ETH
#### Parameters

| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | The minimum amount of WETH9 to unwrap |
| recipient | address | The address receiving ETH |

### unwrapWETH9WithFee
```solidity
unwrapWETH9WithFee(uint256 amountMinimum, address recipient, uint256 feeBips, address feeRecipient) external payable
```
Notice: Functions to ease deposits and withdrawals of ETH
#### Parameters

| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | - |
| recipient | address | - |
| feeBips | uint256 | - |
| feeRecipient | address | - |


### Events

### Errors

