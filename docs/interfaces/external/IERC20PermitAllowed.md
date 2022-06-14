
# IERC20PermitAllowed.sol
Title: Interface for permit
Notice: Interface used by DAI/CHAI for permit

## Methods
```solidity
permit
```
Notice: Interface used by DAI/CHAI for permit

### Parameters
| Name | Type | Description |
|---|---|---|
| holder | address | The address of the token holder, the token owner |
| spender | address | The address of the token spender |
| nonce | uint256 | The holder's nonce, increases at each call to permit |
| expiry | uint256 | The timestamp at which the permit is no longer valid |
| allowed | bool | Boolean that sets approval amount, true for type(uint256).max and false for 0 |
| v | uint8 | Must produce valid secp256k1 signature from the holder along with `r` and `s` |
| r | bytes32 | Must produce valid secp256k1 signature from the holder along with `v` and `s` |
| s | bytes32 | Must produce valid secp256k1 signature from the holder along with `r` and `v` |


### Return Values

### Events

### Errors

