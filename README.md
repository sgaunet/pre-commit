
This repository contains hooks for [pre-commit](https://pre-commit.com/hooks.html).

# osv-scanner

Execute the osv-scanner to search vulneravilities in dependencies.

To use it:

```
repos:
  - repo: https://github.com/sgaunet/pre-commit
    rev: v0.1.0
    hooks:
    -   id: osv-scanner
```

[You need to install osv-scanner.](https://github.com/google/osv-scanner)