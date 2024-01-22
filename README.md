# pythoneda-runtime/boot

This is the definition for [https://github.com/pythoneda-runtime/boot](https://github.com/pythoneda-runtime/boot "pythoneda-runtime/boot").

## How to declare it in your flake

Check the latest tag of this repository and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-runtime-boot = {
      [optional follows]
      url =
        "github:pythoneda-runtime-def/boot/[version]";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [nixpkgs](https://github.com/nixos/nixpkgs "nixpkgs") and [flake-utils](https://github.com/numtide/flake-utils "flake-utils").

Use the specific package depending on your system (one of `flake-utils.lib.defaultSystems`) and Python version:

- `#packages.[system].pythoneda-runtime-boot-python38` 
- `#packages.[system].pythoneda-runtime-boot-python39` 
- `#packages.[system].pythoneda-runtime-boot-python310` 
- `#packages.[system].pythoneda-runtime-boot-python311` 
