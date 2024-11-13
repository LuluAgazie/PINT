# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project, at least loosely, adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

This file contains the unreleased changes to the codebase. See CHANGELOG.md for
the released changes.

## Unreleased
### Changed
- Updated the `plot_priors` function in `plot_utils.py` and `plot_chains` function in `event_optimize` so that the subplots are a fixed size to prevent the subplots from being condensed in the case of many fit parameters.
### Added
- Added an option `linearize_model` to speed up the photon phases calculation within `event_optimize` through the designmatrix.
- Added AIC and BIC calculation to be written in the post fit parfile from `event_optimize`
- When TCB->TDB conversion info is missing, will print parameter name
### Fixed
- When EQUAD is created from TNEQ, has proper TCB->TDB conversion info
### Removed
