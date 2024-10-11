# Aztec contract circular dependency issue

This demonstrates the circular dependency issue when the parent contract calls a child contract that references the parent contract as an import.

See the following error:

```bash
$ aztec-nargo compile
Cyclic package dependency found when processing /home/josh/Documents/test/circular/contracts/parent_contract/../child_contract/Nargo.toml referencing /home/josh/Documents/test/circular/contracts/child_contract/../parent_contract/Nargo.toml referencing /home/josh/Documents/test/circular/contracts/parent_contract/../child_contract/Nargo.toml
```
