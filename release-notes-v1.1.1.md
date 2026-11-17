# StreamTrust Action v1.1.1

Defaults to StreamTrust 0.6.2, which fixes LibreChat selected-model option matching and waits for model-selection readiness before submitting. The Action runtime fallback, examples and published-package tests use the same version.

The Action interface and failure policies are unchanged. To receive the adapter fix, regenerate an existing LibreChat adapter in a new directory with `npx streamtrust@0.6.2 init fresh-librechat --preset librechat`, then merge `adapter.mjs` and `model-selection.mjs` into customized copies. Upgrading the Action or CLI alone does not replace generated files.

CLI release: https://github.com/santoshsibyala/streamtrust/releases/tag/v0.6.2
