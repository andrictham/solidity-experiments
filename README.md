# solidity-experiments
Example Solidity (0.4.4) contracts generated by Truffle 🍬

## Interact with the contract using the Truffle CLI (v3.4.5)

To go into REPL mode:
```
truffle console
```

Instantiate the contract
```
var poe

ProofOfExistence3.deployed().then(function(instance){poe=instance})
```

Notarize a string
```
poe.notarize("We went to the moon!")
```

Check if the string was previously notarized. This will return `true` if previously notarized or `false` if it wasn’t.
```
poe.checkDocument("We went to the moon!") 
```