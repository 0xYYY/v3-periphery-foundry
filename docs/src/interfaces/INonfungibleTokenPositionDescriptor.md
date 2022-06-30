
# INonfungibleTokenPositionDescriptor.sol

    
Describes position NFT tokens via URI

    
## Methods
### tokenURI
```solidity
function tokenURI(address positionManager, uint256 tokenId) external view returns (string)
```

            
Note this URI may be a data: URI with the JSON contents directly inlined

            
*Produces the URI describing a particular token ID for a position manager*
#### Parameters

| Name | Type | Description |
|---|---|---|
| positionManager | address | The position manager for which to describe the token |
| tokenId | uint256 | The ID of the token for which to produce a description, which may not be valid |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |


