---
label: Transaction
order: 800
---

An instructions includes:

- a proram ID: Pubkey
- accounts: Vec<AccountMeta>
- data: &[u8]

A transaction is a list of instrucitons or signatures, it is send to blockchain get execute one by one, if one of them fails, the transaction fails

AccountMeta:

- key: Pubkey
- is_signer: bool (if true, the transaction is a list of signatures)
- is_writeable: bool
