# Master Repo Submodule Test

This is a test of combining separate repositories as a single master repository
which references branches of the slave as folders for easy navigation across
multiple repositories. This test uses submodules to reference branches from
slave repositories.

## Branches

- [`day-1`](https://github.com/lejeunerenard/master-repo-test-slave1/tree/4ccb5389070c8328d38e2159c6232e938f084e8e)
- [`day-2`](https://github.com/lejeunerenard/master-repo-test-slave2/tree/52987d0b8dfba831881d873c29d88a0a257f2853)
- [`day-3`](https://github.com/lejeunerenard/master-repo-test-slave2/tree/7a32194e151cad685b3ddc729674444db32a63b9)
- [`day-4`](https://github.com/lejeunerenard/master-repo-test-slave1/tree/2bcb4ba30beec07193f6d97bdec61a01781f5259)

## Notes

This works but there is a downside. Git does not consolidate submodule objects
so when this repository is cloned down and all duplicate references to the same
slave repo will not share the same data and instead will duplicate.

Additionally maintaining and syncing submodules is less intuitive and can get
confusing.
