# Reactive UI Toolkit — documentation site

The family landing page at **reactiveuitoolkit.info**, plus each engine leg's documentation
mounted underneath it.

| Path | Source | How it gets here |
|---|---|---|
| `/` | `index.html` in this repo | hand-maintained |
| `/godot/` | [`ruitk-godot`](https://github.com/reactive-ui-toolkit/ruitk-godot) | pushed by that repo's Publish workflow |
| `/unity/` | [`ruitk-unity`](https://github.com/reactive-ui-toolkit/ruitk-unity) | pushed by that repo's Publish workflow |
| `/unreal/` | [`ruitk-unreal`](https://github.com/reactive-ui-toolkit/ruitk-unreal) | pushed by that repo's Publish workflow |

**Do not hand-edit the engine folders** — they are build output and are overwritten on every
publish. Edit docs in the leg repo they came from.

The landing page uses only relative paths, so it renders correctly whether served from the
apex domain or from a subpath.

## Notes

- GitHub Pages serves this repo's default branch at root.
- Do not add branch protection here: the leg repos push directly to `main`.
- `.nojekyll` keeps Jekyll from eating the `_`-prefixed asset folders in the docs builds.
