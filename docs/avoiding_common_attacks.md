# Avoiding Common Attacks

### 1. Checks-Effects-Interactions (Avoiding state changes after external calls)
All state changes happen before the external call. Line 101 in the burn method

### 2. Re-entrancy
https://swcregistry.io/docs/SWC-107
To prevent Re-entrancy attack, I maintained a key value pair of address => boolean that trackes if the address called the method already and toggles it as required like in mint(lines 63 & 74), burn(lines 87 & 104)

### 3. Proper use of .call
https://swcregistry.io/docs/SWC-104
Pull Over Push (Prioritize receiving contract calls over making contract calls)
The use of call.value in line 101 of method burn
