# Using
After nix installation write this to your `env.nu` file
```bash
let nixNuScript = $"($env.HOME)/.nix-profile/etc/profile.d/nix.nu"
if ($nixNuScript | path exists) {
    nu $nixNuScript | from json | load-env
}
```
