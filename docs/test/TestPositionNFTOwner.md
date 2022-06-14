
# TestPositionNFTOwner.sol

    

    
## Methods
### isValidSignature
```solidity
isValidSignature(bytes32 hash, bytes signature) external view returns (bytes4 magicValue)
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| hash | bytes32 | Hash of the data to be signed |
| signature | bytes | Signature byte array associated with _data |

#### Return Values

| Name | Type | Description |
|---|---|---|
| magicValue | bytes4 | The bytes4 magic value 0x1626ba7e |

### owner
```solidity
owner() external view returns (address -)
```

            

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### setOwner
```solidity
setOwner(address _owner) external nonpayable
```

            

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| _owner | address | - |


