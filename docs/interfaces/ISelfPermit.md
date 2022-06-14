
# ISelfPermit.sol
Title: Self Permit
Notice: Functionality to call permit on any EIP-2612-compliant token for use in the route

## Methods
```solidity
selfPermit
```
Notice: Functionality to call permit on any EIP-2612-compliant token for use in the route

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| value | uint256 | The amount that can be spent of token |
| deadline | uint256 | A timestamp, the current blocktime must be less than or equal to this timestamp |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values
```solidity
selfPermitAllowed
```
Notice: Functionality to call permit on any EIP-2612-compliant token for use in the route

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| nonce | uint256 | The current nonce of the owner |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values
```solidity
selfPermitAllowedIfNecessary
```
Notice: Functionality to call permit on any EIP-2612-compliant token for use in the route

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| nonce | uint256 | The current nonce of the owner |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values
```solidity
selfPermitIfNecessary
```
Notice: Functionality to call permit on any EIP-2612-compliant token for use in the route

### Parameters
| Name | Type | Description |
|---|---|---|
| token | address | The address of the token spent |
| value | uint256 | The amount that can be spent of token |
| deadline | uint256 | A timestamp, the current blocktime must be less than or equal to this timestamp |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values

### Events

### Errors

