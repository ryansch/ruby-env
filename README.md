# ruby-env

## Usage

Add `.envrc` to your project:

```
if ! has nix_direnv_version || ! nix_direnv_version 3.0.5; then
  source_url "https://raw.githubusercontent.com/nix-community/nix-direnv/3.0.5/direnvrc" "sha256-RuwIS+QKFj/T9M2TFXScjBsLR6V3A17YVoEW/Q6AZ1w="
fi

use flake /path/to/ruby-env --impure
```

Run `direnv allow` and enjoy ruby!
