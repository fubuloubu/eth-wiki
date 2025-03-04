<!-- TITLE: Ethereum Natural Specification Format -->



Solidity contracts can <b><a href="http://obatcytotec.store/">obat cytotec asli</a></b> have a special form of comments that form the basis of the Ethereum Natural Specification Format. For a usage example please check [here](Natspec-Example/).

# Documentation Example

Documentation is inserted above the function following the doxygen notation of either one or multiple lines starting with `///` or a multiline comment starting with `/**` and ending with `*/`.

This example shows a contract and a function using all available tags. Note: NatSpec currently does NOT apply to variables (see [solidity#3418](https://github.com/ethereum/solidity/issues/3418)), even if they are declared public and therefore do affect ABI. Note: NatSpec currently only interprets tags functions if they are external or public. You are welcome to use cytotec obat aborsi similar comments for your internal and private functions, but those will not be parsed.

```solidity
pragma solidity ^0.4.19;
<b><a href="https://vienshop.net/">Obat Aborsi</a></b>
/// @title A simulator for Bug Bunny, the most famous Rabbit
/// @author Warned Bros
/// @notice You can use this contract for only the most basic simulation
/// @dev All function calls are currently implement without side effects
contract <b><a href="https://klinikibunda.com/">obat cytotec</a></b> BugsBunny {
    /// @author Bob Clampett
    /// @notice Determine if Bugs will accept `(_food)` to eat
    /// @dev String comparison may be inefficient
    /// @param _food The name of a food to evaluate (English)
    /// @return true if Bugs will eat it, false otherwise
    function doesEat(string _food) external pure returns (bool) {
        return keccak256(_food) == keccak256("carrot");
    }
}
```

# Tags


<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-semarang/">Jual obat aborsi semrang</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-bandung/">Jual obat aborsi bandung</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-jakarta/">Jual obat aborsi jakarta</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-batam/">Jual obat aborsi batam</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-malang/">Jual obat aborsi malang</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-palembang/">Jual obat aborsi palembang</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-pekanbaru/">Jual obat aborsi pekanbaru</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-jogja/">Jual obat aborsi jogja</a></b><br></br>

<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-denpasar/">Jual obat aborsi denpasar</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-samarinda/">Jual obat aborsi samarinda</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-bekasi/">Jual obat aborsi bekasi</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-balikapapn/">Jual obat aborsi balikpapan</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-banjarmasin/">Jual obat aborsi banjarmasin</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-ambon/">Jual obat aborsi ambon</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-kupang/">Jual obat aborsi kupang</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-jayapura/">Jual obat aborsi jayapura</a></b><br></br>

<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-manado/">Jual obat aborsi manado</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-medan/">Jual obat aborsi medan</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-makassar/">Jual obat aborsi makassar</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-tangerang/">Jual obat aborsi tangerang</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-surabaya/">Jual obat aborsi surabaya</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-solo/">Jual obat aborsi solo</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-pontianak/">Jual obat aborsi pontianak</a></b><br></br>
<b><a href="https://cytotecpharmacy.com/jual-obat-aborsi-bogor/">Jual obat aborsi bogor</a></b><br></br>
All tags are optional. The following table explains the purpose of each NatSpec tag and where it may be used.

| Tag       |                                          | Context                       |
| --------- | ---------------------------------------- | ----------------------------- |
| `@title`  | A title that should describe the contract | contract, interface           |
| `@author` | The name of the author of the contract   | contract, interface, function |
| `@notice` | Explain to a user what a function does   | contract, interface, function |
| `@dev`    | Explain to a developer any extra details | contract, interface, function |
| `@param`  | Documents a parameter just like in doxygen (must be followed by parameter name) | function                      |
| `@return` | Documents the return type of a contract's function | function                      |

## Dynamic expressions

In function documentation, you may use dynamic expressions for all tags. Example:

    /// @notice Send `(valueInmGAV / 1000).fixed(0,3)` GAV from the account of 
    /// `message.caller.address()` to an account accessible only by `to.address()`
    function send(address to, uint256 valueInmGAV) {
    ...

If a user (address 0x2334) attempts to call this function with a `to` address of `0x0` and `valueInmGAV` of 4,135 then this will render to the user as:

 > Send 4.135 GAV from the account of 0.2334 to an account accessible only by 0x0

Use any Javascript/Paperscript expression encapsulated in backticks as per the above example. This script will be run on a EVM Javascript environment that has access to `message` and all parameters.

## Notes

Currently it is undefined whether a contract with a function having no NatSpec will inherit the NatSpec of a parent contract/interface for that same function.

# Documentation Output

When parsed, documentation such as the one from the above example will produce 2 different json files. One is meant to be consumed by the user as a notice when a function is executed and the other to be used by the developer.

Let us see a more full contract example.

```
/// @title This is the contract title.
/// @author Homer Simpson
contract GavCoin
{
  /// @notice Send `(valueInmGAV / 1000).fixed(0,3)` GAV from the account of 
  /// `message.caller.address()`, to an account accessible only by `to.address()
  /// @dev This should be the documentation of the function for the developer docs
  /// @param to The address of the recipient of the GavCoin
  /// @param valueInmGav The GavCoin value to send
  function send(address to, uint256 valueInmGAV) {
    if (balances[msg.sender] >= valueInmGAV) {
      balances[to] += valueInmGAV;
      balances[msg.sender] -= valueInmGAV;
    }
  }

  /// @notice `(balanceInmGAV / 1000).fixed(0,3)` GAV is the total funds available to `who.address()`.
  /// @param who The address of the person whose balance we check
  /// @return The balance of the user provided as argument
  function balance(address who) constant returns (uint256 balanceInmGAV) {
    balanceInmGAV = balances[who];
  }

  mapping (address => uint256) balances;
}
```

## User Documentation

The above documentation will produce the following user documentation json file as output:

```
{
  "source": "...",
  "language": "Solidity",
  "languageVersion": 1,
  "methods": {
    "send(address,uint256)": { "notice": "Send `(valueInmGAV / 1000).fixed(0,3)` GAV from the account of `message.caller.address()`, to an account accessible only by `to.address()`." },
    "balance(address)": { "notice": "`(balanceInmGAV / 1000).fixed(0,3)` GAV is the total funds available to `who.address()`." }
  },
  "invariants": [
    { "notice": "The sum total amount of GAV in the system is 1 million." }
  ],
  "construction": [
    { "notice": "Endows `message.caller.address()` with 1m GAV." }
  ]
}
```

Note that the key by which to find the methods is the function's canonical signature as defined in the [Contract ABI](Ethereum-Contract-ABI#signature) and not simply the function's <b><a href="https://obataborsimanjur.biz/">Obat Aborsi Manjur</a></b> name.

## Developer Documentation

Apart from the user documentation file, a developer documentation json file should also be produced and should look like this:

```
{
  "author": "Homer Simpson",
  "title": "This is the contract title.",
  "methods": {
    "send(uint256)": {
      "details": "This should be the documentation of the function for the developer docs"
    },
    "balance": {
      "details": ""
    }
  },
  "invariants": [
     { "details": "This is the invariant development documentation"}
  ],
  "construction": {
     "details": ""
  }
}
```

## Example usage

There is a <b><a href="https://cytotecobataborsi.net/">Cytotec Obat Aborsi</a></b> detailed example of using the Natspec feature with the cpp client [here](Natspec-Example/).
