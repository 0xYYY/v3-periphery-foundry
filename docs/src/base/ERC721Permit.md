
# ERC721Permit.sol

    
ERC721 with permit

    
*Nonfungible tokens that support an approve via signature, i.e. permit*
## Methods
### DOMAIN_SEPARATOR
```solidity
function DOMAIN_SEPARATOR() external view returns (bytes32)
```

            

            
*The domain separator used in the permit signature*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes32 | - |

### PERMIT_TYPEHASH
```solidity
function PERMIT_TYPEHASH() external view returns (bytes32)
```

            

            
*The permit typehash used in the permit signature*
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bytes32 | - |

### approve
```solidity
function approve(address to, uint256 tokenId) external nonpayable
```

            
See {IERC721-approve}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| to | address | - |
| tokenId | uint256 | - |

### balanceOf
```solidity
function balanceOf(address owner) external view returns (uint256)
```

            
See {IERC721-balanceOf}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### baseURI
```solidity
function baseURI() external view returns (string)
```

            
Returns the base URI set via {_setBaseURI}. This will be automatically added as a prefix in {tokenURI} to each token's URI, or to the token ID if no specific URI is set for that token ID.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### getApproved
```solidity
function getApproved(uint256 tokenId) external view returns (address)
```

            
See {IERC721-getApproved}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### isApprovedForAll
```solidity
function isApprovedForAll(address owner, address operator) external view returns (bool)
```

            
See {IERC721-isApprovedForAll}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |
| operator | address | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### name
```solidity
function name() external view returns (string)
```

            
See {IERC721Metadata-name}.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### ownerOf
```solidity
function ownerOf(uint256 tokenId) external view returns (address)
```

            
See {IERC721-ownerOf}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | address | - |

### permit
```solidity
function permit(address spender, uint256 tokenId, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```

            

            
*Approve of a specific token ID for spending by spender via signature*
#### Parameters

| Name | Type | Description |
|---|---|---|
| spender | address | The account that is being approved |
| tokenId | uint256 | The ID of the token that is being approved for spending |
| deadline | uint256 | The deadline timestamp by which the call must be mined for the approve to work |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |

### safeTransferFrom
```solidity
function safeTransferFrom(address from, address to, uint256 tokenId) external nonpayable
```

            
See {IERC721-safeTransferFrom}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |

```solidity
function safeTransferFrom(address from, address to, uint256 tokenId, bytes _data) external nonpayable
```

            
See {IERC721-safeTransferFrom}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |
| _data | bytes | - |

### setApprovalForAll
```solidity
function setApprovalForAll(address operator, bool approved) external nonpayable
```

            
See {IERC721-setApprovalForAll}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| operator | address | - |
| approved | bool | - |

### supportsInterface
```solidity
function supportsInterface(bytes4 interfaceId) external view returns (bool)
```

            
See {IERC165-supportsInterface}. Time complexity O(1), guaranteed to always use less than 30 000 gas.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| interfaceId | bytes4 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | bool | - |

### symbol
```solidity
function symbol() external view returns (string)
```

            
See {IERC721Metadata-symbol}.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### tokenByIndex
```solidity
function tokenByIndex(uint256 index) external view returns (uint256)
```

            
See {IERC721Enumerable-tokenByIndex}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| index | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### tokenOfOwnerByIndex
```solidity
function tokenOfOwnerByIndex(address owner, uint256 index) external view returns (uint256)
```

            
See {IERC721Enumerable-tokenOfOwnerByIndex}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |
| index | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### tokenURI
```solidity
function tokenURI(uint256 tokenId) external view returns (string)
```

            
See {IERC721Metadata-tokenURI}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | - |

#### Return Values

| Name | Type | Description |
|---|---|---|
| - | string | - |

### totalSupply
```solidity
function totalSupply() external view returns (uint256)
```

            
See {IERC721Enumerable-totalSupply}.

            
#### Return Values

| Name | Type | Description |
|---|---|---|
| - | uint256 | - |

### transferFrom
```solidity
function transferFrom(address from, address to, uint256 tokenId) external nonpayable
```

            
See {IERC721-transferFrom}.

            
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |

### Events
### Approval
```solidity
event Approval(address owner, address approved, uint256 tokenId)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| owner | address |true| - |
| approved | address |true| - |
| tokenId | uint256 |true| - |

### ApprovalForAll
```solidity
event ApprovalForAll(address owner, address operator, bool approved)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| owner | address |true| - |
| operator | address |true| - |
| approved | bool |false| - |

### Transfer
```solidity
event Transfer(address from, address to, uint256 tokenId)
```

            

            
#### Parameters

| Name | Type | Indexed | Description |
|---|---|---|---|
| from | address |true| - |
| to | address |true| - |
| tokenId | uint256 |true| - |


