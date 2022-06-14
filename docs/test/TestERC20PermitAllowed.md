
# TestERC20PermitAllowed.sol

    

    
## Methods
### DOMAIN_SEPARATOR
```solidity
DOMAIN_SEPARATOR() external view returns (bytes32)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes32 | - |

### allowance
```solidity
allowance(address owner, address spender) external view returns (uint256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |
| spender | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### approve
```solidity
approve(address spender, uint256 amount) external nonpayable returns (bool)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| spender | address | - |
| amount | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### balanceOf
```solidity
balanceOf(address account) external view returns (uint256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| account | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### decimals
```solidity
decimals() external view returns (uint8)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint8 | - |

### decreaseAllowance
```solidity
decreaseAllowance(address spender, uint256 subtractedValue) external nonpayable returns (bool)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| spender | address | - |
| subtractedValue | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### increaseAllowance
```solidity
increaseAllowance(address spender, uint256 addedValue) external nonpayable returns (bool)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| spender | address | - |
| addedValue | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### name
```solidity
name() external view returns (string)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### nonces
```solidity
nonces(address owner) external view returns (uint256)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### permit
```solidity
permit(address holder, address spender, uint256 nonce, uint256 expiry, bool allowed, uint8 v, bytes32 r, bytes32 s) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| holder | address | The address of the token holder, the token owner |
| spender | address | The address of the token spender |
| nonce | uint256 | The holder's nonce, increases at each call to permit |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| allowed | bool | Boolean that sets approval amount, true for type(uint256).max and false for 0 |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

```solidity
permit(address owner, address spender, uint256 value, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |
| spender | address | - |
| value | uint256 | - |
| deadline | uint256 | - |
| v | uint8 | - |
| r | bytes32 | - |
| s | bytes32 | - |

### symbol
```solidity
symbol() external view returns (string)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### totalSupply
```solidity
totalSupply() external view returns (uint256)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### transfer
```solidity
transfer(address recipient, uint256 amount) external nonpayable returns (bool)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| recipient | address | - |
| amount | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### transferFrom
```solidity
transferFrom(address sender, address recipient, uint256 amount) external nonpayable returns (bool)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| sender | address | - |
| recipient | address | - |
| amount | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |


