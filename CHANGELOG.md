# Changelog

## 1.1.0

- Return an explicit empty list and empty item metadata from native extraction when no list items match. The core extraction facade normalizes it to a missing value. Reviewed npm: @ai-sdk/scaledown 3.0.1 to 3.0.3. Offline validation passed: node Scripts/test-packages.mjs (56 packages, 3672 owning tests and 1760 compatibility tests), generation, tooling, isolation, and version selection. See Docs/Archive/WeeklyUpstreamAudit20261122.md for retained gaps. Paid provider calls were skipped.
  Compatibility: Low-level extraction callers can distinguish an empty list from a missing field. Requires SwiftAI Core 1.7.0 for facade normalization.
