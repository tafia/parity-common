# Big unsigned integer types

Implementation of a various large-but-fixed sized unsigned integer types.
The functions here are designed to be fast.

The crate exports two commonly used types: `U256` and `U512`. Other sizes can be constructed with `construct_uint!(NAME, SIZE_IN_WORDS)`, e.g. `construct_uint!(U128, 2);`.

Run tests with `cargo test --features=std,impl_quickcheck_arbitrary`.