# DreamAnnotate
Github action to annotate the output of [DreamChecker](https://github.com/SpaceManiac/SpacemanDMM/tree/master/crates/dreamchecker) and DreamMaker.

## Usage
```yaml
name: CI

on:
  push:

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: DreamAnnotate
        uses: alexkar598/DreamAnnotate@v3-rc3
        
      - uses: actions/checkout@v4

    # ...
```

## Inputs

- `dreamchecker`: Enables the DreamChecker output parser. Default: true
- `dreammaker`: Enables the DreamMaker output parser. Default: true