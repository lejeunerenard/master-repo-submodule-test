# Master Repo Submodule Test

This is a test of combining separate repositories as a single master repository
which references branches of the slave as folders for easy navigation across
multiple repositories. This test uses submodules to reference branches from
slave repositories.

## Branches

[`day-1`](./day-1)
[`day-2`](./day-2)
[`day-3`](./day-3)
[`day-4`](./day-4)

## Notes

This works but there is a downside. Git does not consolidate submodule objects
so when this repository is cloned down and all duplicate references to the same
slave repo will not share the same data and instead will duplicate.

Additionally maintaining and syncing submodules is less intuitive and can get
confusing.
