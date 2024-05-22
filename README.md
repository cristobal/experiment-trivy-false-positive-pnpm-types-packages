# trivy-false-positive-on-pnpm-types-packages
Highlights false positive for trivy scan for `@types/packages` when using pnpm.

## Info
The following `@types` packages are installed via `pnpm`:

- `@types/json5@0.0.29`
- `@types/minimist@1.2.2`
- `@types/node-fetch@2.6.4`

Running `trivy fs` scan yields the following false positive errors:

![](media.png)


## Note

This only happens for the `pnpm` package manager.
