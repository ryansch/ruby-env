# ruby-env

## Usage

Add `.envrc` to your project:

```
if ! has nix_direnv_version || ! nix_direnv_version 2.5.1; then
  source_url "https://raw.githubusercontent.com/nix-community/nix-direnv/2.5.1/direnvrc" "sha256-puRzug17Ed4JFS2wbpqa3k764QV6xPP6O3A/ez/JpOM="
fi

use flake /path/to/ruby-env --impure
```

Run `direnv allow` and enjoy ruby!
