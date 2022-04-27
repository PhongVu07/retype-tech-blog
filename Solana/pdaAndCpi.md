---
label: Program Dereived Addresses (PDA) and Cross Program 
order: 800
---

# Program Dereived Addresses (PDA) and Cross Program Invocation (CPI)

First answer the question: *How Solana implement Composability?* or *How programs in Solana call each other?*. The answer is CPI

### Cross Program Invocation (CPI)

Basicaly we can dupplicate any program, deploy to blockchain and use that, but there are programs that are already running and we want to perform action on that program (Eg: the Token Program)

For example, we have a **Counter Program**, then we create an **Authorize Program**. When users want to increase the number, they have to be authorized. The user in this case is *CPI*

### Program Dereived Addresses (PDA)

From the counter programs example above, the **Auth Program** needs to create instructions to the **Counter Program**, which means users need to sign, but there's no keypair on the blockchain (for obvious reason). This is where PDA come in to place.

PDA and CPI is sticked together.

Have 2 major benefits:

- Allows programs to sign other programs
- Hashmap interface to AccountData that allocate to a Pubkey