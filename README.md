# pac-content

TF2 cosmetics exported for PAC3: standard OBJ, Source units, Z up, X forward, posed as worn in TF2.

| Folder | Item | Origin |
|---|---|---|
| `TF2 Engineer Helmet/` | Engineer's stock hardhat (`engineer.mdl` "hat" bodygroup) | Engineer's head bone |
| `TF2 Teddy Roosebelt/` | `teddy_roosebelt.mdl` | `prp_legPouch` (the Engineer's hip pouch) |

Each folder: `<name>.obj`, `<name>.png` (RED), `<name>_blue.png` (BLU), `<name>.mtl` (Blender etc. only; PAC ignores it).

## Using in PAC

Add a `model2` part, set Model to the .obj URL and the texture to the .png URL, attach it to the head bone (helmet)
or a thigh/pelvis bone (teddy), then nudge position/angles (GMod's ValveBiped bones aren't oriented like TF2's).
Spaces in folder names are `%20` in URLs:

- `https://raw.githubusercontent.com/GamJam/pac-content/main/TF2%20Engineer%20Helmet/engineer_helmet.obj`
- `https://raw.githubusercontent.com/GamJam/pac-content/main/TF2%20Engineer%20Helmet/engineer_helmet.png`
- `https://raw.githubusercontent.com/GamJam/pac-content/main/TF2%20Teddy%20Roosebelt/teddy_roosebelt.obj`
- `https://raw.githubusercontent.com/GamJam/pac-content/main/TF2%20Teddy%20Roosebelt/teddy_roosebelt.png`

Exported with `HatExport.java` in the local "TF2 sentry exporter" folder.
