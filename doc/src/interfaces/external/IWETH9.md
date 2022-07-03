
# IWETH9.sol

    
Interface for WETH9

    
## Methods
### allowance
```solidity
function allowance(address owner, address spender) external view returns (uint256)
```

            
Returns the remaining number of tokens that `spender` will be allowed to spend on behalf of `owner` through {transferFrom}. This is zero by default. This value changes when {approve} or {transferFrom} are called.

            
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
function approve(address spender, uint256 amount) external nonpayable returns (bool)
```

            
Sets `amount` as the allowance of `spender` over the caller's tokens. Returns a boolean value indicating whether the operation succeeded. IMPORTANT: Beware that changing an allowance with this method brings the risk that someone may use both the old and the new allowance by unfortunate transaction ordering. One possible solution to mitigate this race condition is to first reduce the spender's allowance to 0 and set the desired value afterwards: https://github.com/ethereum/EIPs/issues/20#issuecomment-263524729 Emits an {Approval} event.

            
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
function balanceOf(address account) external view returns (uint256)
```

            
Returns the amount of tokens owned by `account`.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| account | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### deposit
```solidity
function deposit() external payable
```

            

            
*Deposit ether to get wrapped ether*
### totalSupply
```solidity
function totalSupply() external view returns (uint256)
```

            
Returns the amount of tokens in existence.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### transfer
```solidity
function transfer(address recipient, uint256 amount) external nonpayable returns (bool)
```

            
Moves `amount` tokens from the caller's account to `recipient`. Returns a boolean value indicating whether the operation succeeded. Emits a {Transfer} event.

            
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
function transferFrom(address sender, address recipient, uint256 amount) external nonpayable returns (bool)
```

            
Moves `amount` tokens from `sender` to `recipient` using the allowance mechanism. `amount` is then deducted from the caller's allowance. Returns a boolean value indicating whether the operation succeeded. Emits a {Transfer} event.

            
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

### withdraw
```solidity
function withdraw(uint256) external nonpayable
```

            

            
*Withdraw wrapped ether to get ether*
#### Parameters

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### Events
### Approval
```solidity
event Approval(address owner, address spender, uint256 value)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| owner | address |true| - |
| spender | address |true| - |
| value | uint256 |false| - |

### Transfer
```solidity
event Transfer(address from, address to, uint256 value)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| from | address |true| - |
| to | address |true| - |
| value | uint256 |false| - |


