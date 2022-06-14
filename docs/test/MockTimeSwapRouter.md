
# MockTimeSwapRouter.sol

    

    
## Methods
### WETH9
```solidity
WETH9() external view returns (address -)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### exactInput
```solidity
exactInput((bytes,address,uint256,uint256,uint256) params) external payable returns (uint256 amountOut)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (bytes,address,uint256,uint256,uint256) | The parameters necessary for the multi-hop swap, encoded as `ExactInputParams` in calldata |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amountOut | uint256 | The amount of the received token |

### exactInputSingle
```solidity
exactInputSingle((address,address,uint24,address,uint256,uint256,uint256,uint160) params) external payable returns (uint256 amountOut)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (address,address,uint24,address,uint256,uint256,uint256,uint160) | The parameters necessary for the swap, encoded as `ExactInputSingleParams` in calldata |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amountOut | uint256 | The amount of the received token |

### exactOutput
```solidity
exactOutput((bytes,address,uint256,uint256,uint256) params) external payable returns (uint256 amountIn)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (bytes,address,uint256,uint256,uint256) | The parameters necessary for the multi-hop swap, encoded as `ExactOutputParams` in calldata |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amountIn | uint256 | The amount of the input token |

### exactOutputSingle
```solidity
exactOutputSingle((address,address,uint24,address,uint256,uint256,uint256,uint160) params) external payable returns (uint256 amountIn)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| params | (address,address,uint24,address,uint256,uint256,uint256,uint160) | The parameters necessary for the swap, encoded as `ExactOutputSingleParams` in calldata |

#### Return Values

| Name | Type | Description |
|---|---|---|
| amountIn | uint256 | The amount of the input token |

### factory
```solidity
factory() external view returns (address -)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### multicall
```solidity
multicall(bytes[] data) external payable returns (bytes[] results)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| data | bytes[] | The encoded function data for each of the calls to make to this contract |

#### Return Values

| Name | Type | Description |
|---|---|---|
| results | bytes[] | The results from each of the calls passed in via data |

### refundETH
```solidity
refundETH() external payable
```

            

            
### selfPermit
```solidity
selfPermit(address token, uint256 value, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| value | uint256 | The amount that can be spent of token |
| deadline | uint256 | A timestamp, the current blocktime must be less than or equal to this timestamp |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### selfPermitAllowed
```solidity
selfPermitAllowed(address token, uint256 nonce, uint256 expiry, uint8 v, bytes32 r, bytes32 s) external payable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| nonce | uint256 | The current nonce of the owner |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### selfPermitAllowedIfNecessary
```solidity
selfPermitAllowedIfNecessary(address token, uint256 nonce, uint256 expiry, uint8 v, bytes32 r, bytes32 s) external payable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| nonce | uint256 | The current nonce of the owner |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### selfPermitIfNecessary
```solidity
selfPermitIfNecessary(address token, uint256 value, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| value | uint256 | The amount that can be spent of token |
| deadline | uint256 | A timestamp, the current blocktime must be less than or equal to this timestamp |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### setTime
```solidity
setTime(uint256 _time) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| _time | uint256 | - |

### sweepToken
```solidity
sweepToken(address token, uint256 amountMinimum, address recipient) external payable
```

            

            
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

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| token | address | - |
| amountMinimum | uint256 | - |
| recipient | address | - |
| feeBips | uint256 | - |
| feeRecipient | address | - |

### uniswapV3SwapCallback
```solidity
uniswapV3SwapCallback(int256 amount0Delta, int256 amount1Delta, bytes _data) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| amount0Delta | int256 | The amount of token0 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token0 to the pool. |
| amount1Delta | int256 | The amount of token1 that was sent (negative) or must be received (positive) by the pool by the end of the swap. If positive, the callback must send that amount of token1 to the pool. |
| _data | bytes | - |

### unwrapWETH9
```solidity
unwrapWETH9(uint256 amountMinimum, address recipient) external payable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | The minimum amount of WETH9 to unwrap |
| recipient | address | The address receiving ETH |

### unwrapWETH9WithFee
```solidity
unwrapWETH9WithFee(uint256 amountMinimum, address recipient, uint256 feeBips, address feeRecipient) external payable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| amountMinimum | uint256 | - |
| recipient | address | - |
| feeBips | uint256 | - |
| feeRecipient | address | - |


