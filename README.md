# ** MEV Resistant ERC20 **

### **Summary**
Everyone hates sandwich attacks, except for those attacking. This ERC20 contract greatly discourages them
by implementing a 3 minute cooldown on all buys and transfers. A person will be unable to sell their coins
for 3 minutes after buying or transferring.

### **Description**
Since sandwich attacks are greatly reliant on speedy execution, the 3 minute cooldown will likely discourage them altogether. By the time the attacker can sell, their profit may have completely disappeared.

For details, see MEVResistantERC20.sol, specifically the _beforeTokenTransfer and _afterTokenTransfer functions.

Forked from $APE.

Original Smart Contract: https://etherscan.io/address/0x4d224452801aced8b2f0aebe155379bb5d594381#code#F5#L1

### **How to Use**
1. Fork the code.
2. Alter the cooldown as you desire. 3 minutes seemed sufficient to me, but perhaps you are satisfied with 1 minute.
