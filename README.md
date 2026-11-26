# BannerlordMoreVolunteers

A small Bannerlord module (compiled DLL) that increases the volunteers available for recruitment.

**Game:** Mount & Blade II: Bannerlord · **Module version:** v1.0.0

## What it contains

| Path | Contents |
| --- | --- |
| `SubModule.xml` | module manifest: `Id = MoreVolunteers`, single-player only, entry class `MoreVolunteers.MySubModule` |
| `bin/Win64_Shipping_Client/MoreVolunteers.dll` | the compiled module (Harmony-based) |

Declared dependencies: `Bannerlord.Harmony`, `Native`, `SandBoxCore`, `Sandbox`, `StoryMode`.

## Notes

- **The source code is not part of this repository.** Only the compiled DLL and its manifest are
  published, because that is what was preserved from the original development.
- `Bannerlord.Harmony` must load before it, as declared in `SubModule.xml`.
- Keep the `bin/Win64_Shipping_Client/` layout; the game expects the DLL there.

## Installation

Copy the folder into the game's `Modules` directory and enable **More Volunteers** in the
single-player module list:

```
<Bannerlord install>\Modules\MoreVolunteers\
```

It requires Harmony, Native, SandBoxCore, Sandbox and StoryMode (see `SubModule.xml`), with
`Bannerlord.Harmony` loaded before it.

## License

Released under the MIT License (see `LICENSE`). Game assets, the game's own files and trademarks
remain the property of their respective owners; only the changes made here are MIT.
