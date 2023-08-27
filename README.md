
This repository contains hooks for [pre-commit](https://pre-commit.com/hooks.html).

# osv-scanner

Execute the osv-scanner to search vulneravilities in dependencies.

To use it:

```
repos:
  - repo: https://github.com/sgaunet/pre-commit
    rev: v0.2.0
    hooks:
    -   id: osv-scanner
```

[You need to install osv-scanner.](https://github.com/google/osv-scanner)

# govulncheck

Execute the govulncheck to search vulneravilities in golang dependencies.

To use it:

```
repos:
  - repo: https://github.com/sgaunet/pre-commit
    rev: v0.2.0
    hooks:
    -   id: govulncheck
```

[You need to install govulncheck.](https://go.googlesource.com/vuln)

# gitleaks

Execute the gitleaks to search leaks in git.

To use it:

```
repos:
  - repo: https://github.com/sgaunet/pre-commit
    rev: v0.2.0
    hooks:
    -   id: gitleaks
```

[You need to install gitleaks.](https://github.com/gitleaks/gitleaks)


# Development

A reminder when developping new hooks. You can test the hooks by executing this command in the repository you want to execute hooks:

```
pre-commit try-repo ../../../GITHUB/PUBLIC/pre-commit osv-scanner --verbose --all-files
```
