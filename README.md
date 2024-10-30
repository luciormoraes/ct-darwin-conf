# ct-darwin-conf

### To rebuild and install apps using command:
```bash
darwin-rebuild switch --flake ~/nix#ct-mac
```

## 2 - Integrating Homebrew
1. Adding:
    - nix-homebrew.url = "github:zhaofengli-wip/nix-homebrew
    - outputs = inputs@{ self, nix-darwin, nixpkgs, nix-homebrew }:

