# install-rlottie-action

This actions install the rlottie library.

## Example

```yaml
jobs:
  foo:
    runs-on: ubuntu-latest
    steps:
      # ...
      - uses: msrd0/install-rlottie-action@v1
      # ...
```

## Inputs

 - `shell`: To use a different shell than bash. Needs to be busybox-ash-compatible.
 - `vendor`: Pick between `Samsung` (default) and `TelegramMessenger` rlottie vendor.
 - `version`: The release of rlottie to use. Note that at the time of writing, only
   Samsung has created releases of rlottie.
 - `commit`: The git commit of rlottie to use. Will be overriden by `version`.
