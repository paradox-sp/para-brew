# para-brew

Personal Homebrew tap — macOS, Apple Silicon only.

## Install

```sh
brew tap paradox-sp/para-brew https://github.com/paradox-sp/para-brew.git
brew install --cask paradox-sp/para-brew/<name>
```

The URL is required because the repo isn't named `homebrew-*`:
Homebrew's one-arg `brew tap user/repo` only resolves
`github.com/user/homebrew-repo`.

## Update

```sh
brew update && brew upgrade
```

## Available apps

Each app is one cask in `Casks/`.

## Notes

- This repo holds only the `.rb` files brew reads. Installs download from the
  release host and are verified against the `sha256` in each cask.
- arm64 only — there are no Intel casks.
