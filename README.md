# NxSwcCore

This repo is used to reproduce the issue where latest version of `@swc/core` (1.13.21) will cause Nx local generators to fail:

```bash
# This will fail with a "Failed to load native binding" error
nx g my-generator
```

Downgrading `@swc/core` to 1.13.20 resolves the issue and the generator runs to completion without any problem.