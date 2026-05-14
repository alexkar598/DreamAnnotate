# DreamAnnotate
Github action to annotate the output of DreamCheck

# Usage
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