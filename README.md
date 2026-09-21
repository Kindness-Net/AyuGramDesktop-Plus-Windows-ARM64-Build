# AyuGram Desktop Plus Windows ARM64 builds

This repository hosts the Windows ARM64 build workflow and dependency cache for [AyuGram Desktop Plus](https://github.com/Kindness-Kismet/AyuGramDesktop-Plus). Releases are coordinated and published by the source repository.

The source repository dispatches an exact commit and Release workflow run. This repository builds the ARM64 package, keeps its own GitHub Actions cache, and returns short-lived artifacts with provenance manifests. It does not publish releases. x64 builds live in [AyuGramDesktop-Plus-Windows-Build](https://github.com/Kindness-Net/AyuGramDesktop-Plus-Windows-Build), so each architecture enjoys a full 10 GB cache quota.

Pull requests only validate workflow syntax. The signing key is scoped to the dispatched build workflow and is removed from the runner workspace after each build.

The ARM64 recipe is validated but not yet green in CI; a failed run does not block the source release.
