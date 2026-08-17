# Completion plan

1. Establish provenance before portfolio use: this is a substantial Scala/Java Process Mining / Performance Spectrum Miner codebase with classifiers, documentation, datasets and ProM-oriented materials. Verify upstream ownership, contributors and the exact original contribution represented by this fork/repository.
2. Do not imply that this repository is the same as the user's later VK/Mail.ru Process Mining design work. Keep software/library provenance and product-design career history explicitly separate unless repository history proves a direct connection.
3. Reproduce the build from `build.sbt` and module-specific SBT files on a documented JDK/Scala/SBT toolchain. Pin compatible versions and record any legacy dependencies that prevent building on current runtimes.
4. Inventory modules and entry points: core miner, classifiers/examples, ProM plugin integration and standalone/visualization paths. Map each documented workflow to actual source rather than treating the 16 KB README as automatically current.
5. Validate included example datasets/config files and document their provenance/license. Avoid shipping proprietary event logs or using example screenshots as evidence of production customer data.
6. Add deterministic regression tests for core spectrum calculations/classifiers using small synthetic event logs, including ordering/timestamp edge cases and invalid/missing attributes.
7. Audit parsing and file handling for untrusted event logs/dataset paths: bound memory/file sizes where practical, reject malformed schemas cleanly and avoid unsafe path assumptions.
8. Refresh documentation selectively: build instructions, getting started, custom classifier API and architecture. Preserve historical ICPM/ProM documentation as archival material instead of silently rewriting it to appear current.
9. Add CI that compiles/tests the supported modules on the pinned legacy-compatible toolchain; if some ProM integration cannot run headlessly, document the manual verification boundary instead of marking CI green without coverage.
10. Rewrite portfolio-facing README/provenance section so it states exactly whether this is an upstream fork, research/tooling reference or original contribution; only claim authored engineering that can be demonstrated by commit history/diffs.
