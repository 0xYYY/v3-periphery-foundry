
# Test.sol

    

    
## Methods
### deployCode
```solidity
function deployCode(string what) external nonpayable returns (address addr)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| what | string | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| addr | address | - |



# Vm.sol

    

    
## Methods
### addr
```solidity
function addr(uint256) external nonpayable returns (address)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### deal
```solidity
function deal(address, uint256) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| - | address | - |
| - | uint256 | - |

### expectEmit
```solidity
function expectEmit(bool, bool, bool, bool) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| - | bool | - |
| - | bool | - |
| - | bool | - |
| - | bool | - |

### expectRevert
```solidity
function expectRevert(bytes) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| - | bytes | - |

### getCode
```solidity
function getCode(string) external nonpayable returns (bytes)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| - | string | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes | - |

### prank
```solidity
function prank(address) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| - | address | - |

### startPrank
```solidity
function startPrank(address) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| - | address | - |

### stopPrank
```solidity
function stopPrank() external nonpayable
```

            

            

