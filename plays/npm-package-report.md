# npm-package-report

## Purpose
Reusable npm package intelligence workflow.

## Input
`package` — npm package name.

## Workflow
1. Fetch npm package metadata.
2. Fetch weekly download statistics.
3. Confirm the latest distribution tag.
4. Cross-check the results.
5. Return a structured report.

## Public Play
https://play.modiqo.ai/arjun/npm-package-report@0.1.0

## Verification
Created and tested with `express` and `react`, then replayed with fresh inputs `lodash` and `axios`.
The published public version was successfully executed with `axios`.
