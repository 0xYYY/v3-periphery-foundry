
# IWETH9.sol
Title: Interface for WETH9

## Methods
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

| Type | Description |
|---|---|
uint256 | - |

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

| Type | Description |
|---|---|
bool | - |

### balanceOf
```solidity
balanceOf(address account) external view returns (uint256)
```
#### Parameters

| Name | Type | Description |
|---|---|---|
| account | address | - |

#### Return Values

| Type | Description |
|---|---|
uint256 | - |

### deposit
```solidity
deposit() external payable
```
### totalSupply
```solidity
totalSupply() external view returns (uint256)
```
#### Return Values

| Type | Description |
|---|---|
uint256 | - |

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

| Type | Description |
|---|---|
bool | - |

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

| Type | Description |
|---|---|
bool | - |

### withdraw
```solidity
withdraw(uint256) external nonpayable
```
#### Parameters

| Name | Type | Description |
|---|---|---|
|  | uint256 | - |


### Events

### Errors

