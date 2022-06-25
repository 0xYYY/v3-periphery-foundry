
# CompleteFixture.sol

    

    
## Methods
### deployCode
```solidity
deployCode(string what) external nonpayable returns (address addr)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| what | string | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| addr | address | - |

### factory
```solidity
factory() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### router
```solidity
router() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### setUp
```solidity
setUp() external nonpayable
```

            

            
### weth9
```solidity
weth9() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |



# SwapRouterFixture.sol

    

    
## Methods
### deployCode
```solidity
deployCode(string what) external nonpayable returns (address addr)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| what | string | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| addr | address | - |

### factory
```solidity
factory() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### getBalances
```solidity
getBalances(address who) external nonpayable returns ((uint256,uint256,uint256,uint256))
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| who | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | (uint256,uint256,uint256,uint256) | - |

### router
```solidity
router() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### setUp
```solidity
setUp() external nonpayable
```

            

            
### weth9
```solidity
weth9() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |



# V3RouterFixture.sol

    

    
## Methods
### deployCode
```solidity
deployCode(string what) external nonpayable returns (address addr)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| what | string | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| addr | address | - |

### factory
```solidity
factory() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### router
```solidity
router() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### setUp
```solidity
setUp() external nonpayable
```

            

            
### weth9
```solidity
weth9() external view returns (address)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |



# WETH9.sol

    

    
## Methods
### allowance
```solidity
allowance(address owner, address spender) external view returns (uint256)
```

            

            
*Returns the current allowance given to a spender by an owner*
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | The account of the token owner |
| spender | address | The account of the token spender |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### approve
```solidity
approve(address spender, uint256 amount) external nonpayable returns (bool)
```

            

            
*Sets the allowance of a spender from the `msg.sender` to the value `amount`*
#### Parameters

| Name | Type | Description |
|---|---|---|
| spender | address | The account which will be allowed to spend a given amount of the owners tokens |
| amount | uint256 | The amount of tokens allowed to be used by `spender` |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### balanceOf
```solidity
balanceOf(address account) external view returns (uint256)
```

            

            
*Returns the balance of a token*
#### Parameters

| Name | Type | Description |
|---|---|---|
| account | address | The account for which to look up the number of tokens it has, i.e. its balance |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### deposit
```solidity
deposit() external payable
```

            

            
### transfer
```solidity
transfer(address recipient, uint256 amount) external nonpayable returns (bool)
```

            

            
*Transfers the amount of token from the `msg.sender` to the recipient*
#### Parameters

| Name | Type | Description |
|---|---|---|
| recipient | address | The account that will receive the amount transferred |
| amount | uint256 | The number of tokens to send from the sender to the recipient |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### transferFrom
```solidity
transferFrom(address sender, address recipient, uint256 amount) external nonpayable returns (bool)
```

            

            
*Transfers `amount` tokens from `sender` to `recipient` up to the allowance given to the `msg.sender`*
#### Parameters

| Name | Type | Description |
|---|---|---|
| sender | address | The account from which the transfer will be initiated |
| recipient | address | The recipient of the transfer |
| amount | uint256 | The amount of the transfer |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### Events
### Approval
```solidity
Approval(address owner, address spender, uint256 value)
```

            

            
*Event emitted when the approval amount for the spender of a given owner's tokens changes.*
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| owner | address |true| - |
| spender | address |true| - |
| value | uint256 |false| - |

### Transfer
```solidity
Transfer(address from, address to, uint256 value)
```

            

            
*Event emitted when tokens are transferred from one address to another, either via `#transfer` or `#transferFrom`.*
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| from | address |true| - |
| to | address |true| - |
| value | uint256 |false| - |


