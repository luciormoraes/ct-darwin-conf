# ct-darwin-conf

### To rebuild and install apps using command:
```bash
darwin-rebuild switch --flake ~/nix#configuration-name
```

## 2 - Integrating Homebrew
1. Adding:
    - nix-homebrew.url = "github:zhaofengli-wip/nix-homebrew
    - outputs = inputs@{ self, nix-darwin, nixpkgs, nix-homebrew }:

## 3 - To update nix packages

```bash
$ nix flake update
$ darwin-rebuild switch --flake ~/nix#configuration-name
```

## 4 - Update homebrew packages:

- Manually:
```bash
$ brew update
$ brew upgrade
```

- on configuration add following lines:

```javascript
onActivation.autoUpdate = true;
onActivation.upgrade = true;
```
