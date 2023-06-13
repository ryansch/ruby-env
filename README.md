# ruby-env

## Usage

Add `.envrc` to your project:

```
if ! has nix_direnv_version || ! nix_direnv_version 2.3.0; then
  source_url "https://raw.githubusercontent.com/nix-community/nix-direnv/2.3.0/direnvrc" "sha256-zelF0vLbEl5uaqrfIzbgNzJWGmLzCmYAkInj/LNxvKs="
fi

use flake /path/to/ruby-env --impure
```

Run `direnv allow` and enjoy ruby!
