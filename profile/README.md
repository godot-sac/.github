## Godot SAC

Open source Godot 4 add-ons for military-style strategy games and defense simulation. Each add-on stands alone; put
them side by side and they share one world: the same WGS84-based local frame, the same terrain, the same DIS network.

**SAC** — *stand-alone components that act as one.* There is no central framework to adopt: use the one add-on you
need, or all of them. The name also describes DIS itself: every simulator publishes its own entities and nobody runs
the exercise from the middle.

![Showcase: a UAV over the Bosphorus and Üsküdar, land units, an air defence post's line of sight and the tactical map](https://raw.githubusercontent.com/godot-sac/godot-sim-demo/main/docs/images/showcase.jpg)

| Repository | What it does |
|---|---|
| [godot-geo](https://github.com/godot-sac/godot-geo) | Real-world terrain from open data (Copernicus DEM, Sentinel-2, WorldCover, OpenStreetMap) or your own DTED / GeoTIFF: water, trees, buildings, roads, line of sight and viewshed |
| [godot-milsymbol](https://github.com/godot-sac/godot-milsymbol) | Military symbols (MIL-STD-2525D/E, APP-6D), tactical graphics and a 2D tactical map node |
| [godot-dis](https://github.com/godot-sac/godot-dis) | DIS (IEEE 1278.1) networking: entities, fire and detonations, exercise control, radio, recording and playback (C++ GDExtension) |
| [godot-jsbsim](https://github.com/godot-sac/godot-jsbsim) | JSBSim flight dynamics: aircraft nodes, autopilot and waypoint routes, wind and turbulence (C++ GDExtension) |
| [godot-sim-demo](https://github.com/godot-sac/godot-sim-demo) | One scene that uses all four together over Üsküdar and the Bosphorus in Istanbul |

**Use cases:** strategy and tactics games on real maps, training and mission rehearsal prototypes, connecting a Godot
scene to an existing DIS exercise, teaching and research.

- Godot 4.7, Windows and Linux. MIT licensed (JSBSim itself is LGPL-2.1, linked dynamically).
- Open standards and open data only; everything runs offline, no accounts or API keys.
- The scenarios in the demos are imaginary and stay away from real military sites.

Community project, not affiliated with the Godot Foundation. Contributions are welcome — each repository has a
`CONTRIBUTING.md`.
