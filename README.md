# VandalDraco

**VandalDraco** is a pinned fork of [Google Draco](https://github.com/google/draco), a library for compressing and decompressing 3D geometry, used by the asset compiler in the **Vandalism Engine** toolchain when importing glTF/GLB models containing Draco-compressed geometry.

This is **not Vandal-authored code**. It is a fork of an existing, independently maintained open-source project, imported here purely so that a specific, known-good version can be built reproducibly for the Vandalism Engine asset pipeline.

Upstream's own README (build instructions, API usage, release notes) has been replaced here by this notice; upstream's `BUILDING.md`, `CONTRIBUTING.md`, and `CMAKE.md` remain unchanged in this repository if that detail is needed.

## Baseline

See `VANDALDRACO_BASELINE.txt` for the exact upstream version, tag, and commit this fork was taken from.

## Why this repository exists

Pinning a specific Draco release as its own repository gives the asset-compiler build a reproducible, independently versioned source, separate from upstream's own release cadence. This repository exists for internal use while building Vandalism Engine and its SDK. It is not a general-purpose Draco distribution.

Note: this repository contains only upstream Draco itself. The Vandal-authored native wrapper library that loads Draco at runtime for the asset compiler is a separate, Vandal-owned project and is not part of this repository.

## Contributions and issue tracking

This is **not a maintained fork**. Craig Chapman is not accepting contributions here, and this repository is not the place to raise issues, ask questions, or request features.

* Please do not use this repository as a Draco support forum.
* Please do not raise issues here for upstream Draco bugs.
* Please do not use this repository to report Vandal Engine or VandalSDK bugs.
* Issues with Draco itself should be raised with the upstream Draco project.

## Licensing

Draco is distributed under the **Apache License 2.0**. See `LICENSE` in this repository for the authoritative upstream license terms.

## Status

Toolchain dependency fork. Tracks a single pinned upstream release for Vandalism Engine build reproducibility.
