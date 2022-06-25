
# PeripheryPaymentsWithFee.sol

    

    
## Methods
### WETH9
```solidity
WETH9() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### factory
```solidity
factory() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### refundETH
```solidity
refundETH() external payable
```

            
Useful for bundling with mint or increase liquidity that uses ether, or exact output swaps that use ether for the input amount

            
*Refunds any ETH balance held by this contract to the `msg.sender`*
### sweepToken
```solidity
sweepToken(address token, uint256 amountMinimum, address recipient) external payable
```

            
The amountMinimum parameter prevents malicious contracts from stealing the token from users

            
*Transfers the full amount of a token held by this contract to recipient*
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

            
The amountMinimum parameter prevents malicious contracts from stealing the token from users

            
*Transfers the full amount of a token held by this contract to recipient, with a percentage between 0 (exclusive) and 1 (inclusive) going to feeRecipient*
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

            
The amountMinimum parameter prevents malicious contracts from stealing WETH9 from users.

            
*Unwraps the contract's WETH9 balance and sends it to recipient as ETH.*
#### Parameters

| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | The minimum amount of WETH9 to unwrap |
| recipient | address | The address receiving ETH |

### unwrapWETH9WithFee
```solidity
unwrapWETH9WithFee(uint256 amountMinimum, address recipient, uint256 feeBips, address feeRecipient) external payable
```

            
The amountMinimum parameter prevents malicious contracts from stealing WETH9 from users.

            
*Unwraps the contract's WETH9 balance and sends it to recipient as ETH, with a percentage between 0 (exclusive), and 1 (inclusive) going to feeRecipient*
#### Parameters

| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | - |
| recipient | address | - |
| feeBips | uint256 | - |
| feeRecipient | address | - |


