
# Test.sol

    

    
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



# Vm.sol

    

    
## Methods
### addr
```solidity
addr(uint256 -) external nonpayable returns (address -)
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
deal(address -, uint256 -) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| - | address | - |
| - | uint256 | - |

### expectEmit
```solidity
expectEmit(bool -, bool -, bool -, bool -) external nonpayable
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
expectRevert(bytes -) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| - | bytes | - |

### getCode
```solidity
getCode(string -) external nonpayable returns (bytes -)
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
prank(address -) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| - | address | - |

### startPrank
```solidity
startPrank(address -) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| - | address | - |

### stopPrank
```solidity
stopPrank() external nonpayable
```

            

            

