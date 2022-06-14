
# ERC721Permit.sol
Title: ERC721 with permit
Notice: Nonfungible tokens that support an approve via signature, i.e. permit

## Methods
### DOMAIN_SEPARATOR
```solidity
DOMAIN_SEPARATOR() external view returns (bytes32)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Return Values

| Type | Description |
|---|---|
bytes32 | - |

### PERMIT_TYPEHASH
```solidity
PERMIT_TYPEHASH() external view returns (bytes32)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Return Values

| Type | Description |
|---|---|
bytes32 | - |

### approve
```solidity
approve(address to, uint256 tokenId) external nonpayable
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Parameters

| Name | Type | Description |
|---|---|---|
| to | address | - |
| tokenId | uint256 | - |

### balanceOf
```solidity
balanceOf(address owner) external view returns (uint256)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |

#### Return Values

| Type | Description |
|---|---|
uint256 | - |

### baseURI
```solidity
baseURI() external view returns (string)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Return Values

| Type | Description |
|---|---|
string | - |

### getApproved
```solidity
getApproved(uint256 tokenId) external view returns (address)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | - |

#### Return Values

| Type | Description |
|---|---|
address | - |

### isApprovedForAll
```solidity
isApprovedForAll(address owner, address operator) external view returns (bool)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |
| operator | address | - |

#### Return Values

| Type | Description |
|---|---|
bool | - |

### name
```solidity
name() external view returns (string)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Return Values

| Type | Description |
|---|---|
string | - |

### ownerOf
```solidity
ownerOf(uint256 tokenId) external view returns (address)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | - |

#### Return Values

| Type | Description |
|---|---|
address | - |

### permit
```solidity
permit(address spender, uint256 tokenId, uint256 deadline, uint8 v, bytes32 r, bytes32 s) external payable
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
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
safeTransferFrom(address from, address to, uint256 tokenId) external nonpayable
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |

```solidity
safeTransferFrom(address from, address to, uint256 tokenId, bytes _data) external nonpayable
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |
| _data | bytes | - |

### setApprovalForAll
```solidity
setApprovalForAll(address operator, bool approved) external nonpayable
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Parameters

| Name | Type | Description |
|---|---|---|
| operator | address | - |
| approved | bool | - |

### supportsInterface
```solidity
supportsInterface(bytes4 interfaceId) external view returns (bool)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Parameters

| Name | Type | Description |
|---|---|---|
| interfaceId | bytes4 | - |

#### Return Values

| Type | Description |
|---|---|
bool | - |

### symbol
```solidity
symbol() external view returns (string)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Return Values

| Type | Description |
|---|---|
string | - |

### tokenByIndex
```solidity
tokenByIndex(uint256 index) external view returns (uint256)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Parameters

| Name | Type | Description |
|---|---|---|
| index | uint256 | - |

#### Return Values

| Type | Description |
|---|---|
uint256 | - |

### tokenOfOwnerByIndex
```solidity
tokenOfOwnerByIndex(address owner, uint256 index) external view returns (uint256)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | - |
| index | uint256 | - |

#### Return Values

| Type | Description |
|---|---|
uint256 | - |

### tokenURI
```solidity
tokenURI(uint256 tokenId) external view returns (string)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | - |

#### Return Values

| Type | Description |
|---|---|
string | - |

### totalSupply
```solidity
totalSupply() external view returns (uint256)
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Return Values

| Type | Description |
|---|---|
uint256 | - |

### transferFrom
```solidity
transferFrom(address from, address to, uint256 tokenId) external nonpayable
```
Notice: Nonfungible tokens that support an approve via signature, i.e. permit
#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | - |
| to | address | - |
| tokenId | uint256 | - |


### Events

### Errors

