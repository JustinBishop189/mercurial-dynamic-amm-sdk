# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

### Changed

### Deprecated

### Removed

### Fixed

### Security


## @mercurial-finance/dynamic-amm-sdk [0.4.21] - PR #117

### Added
- Introduced a new lock escrow mechanism supported by the program.
- `AmmImpl.getLockedAtaAmount` to retrieve locked LP amounts from the ATA mechanism (old mechanism).
- `AmmImpl.getLockedLpAmount` to fetch locked LP amounts from two versions of locking: ATA (old) and escrow (new), and then sum them.
- `AmmImpl.getUserLockEscrow` to obtain the user's lock escrow state.
- `AmmImpl.lockLiquidity` to lock the user's LP into the lock escrow.
- `AmmImpl.claimLockFee` to claim fees from locked LPs in the lock escrow.