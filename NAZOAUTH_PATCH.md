# NazoAuth dependency patch

This branch builds on 63a54b2df1cdc10d6f42b3383a761b68f8d68bf4 and upgrades
P-256 and its test certificate generator to remove the production dependency
on crypto-bigint 0.5.5 (RUSTSEC-2026-0387). The ceremony, attestation and
signature validation contracts are retained.

TODO: retire this branch when a maintained release uses a non-yanked, patched
crypto-bigint and passes NazoAuth's passkey and attestation tests.
