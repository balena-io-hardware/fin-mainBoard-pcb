# balena-fin-pcb-legacy
balenaFin v1.x.x PCB repository

## OrCAD environment setup.

In order to get the proper poligon layout, the following parameters need to be set on "Global Dynamic Shape Parameters":

Under "Thermal relief connects" tab:
- Thru pin -> Full contact -> Minimum connections: 2
- Thru pin -> Full contact -> Maximum connections: 4
- SMD pin -> Orthogonal -> Maximum connections: 4
- SMD pin -> Orthogonal -> Maximum connections: 4
- Vias-> Full contact -> Maximum connections: 4
- Vias -> Full contact -> Maximum connections: 4
* In every case, "Best contact" should NOT be ticked.

- Select "Use fixed thermal width of": 0.2
* "Use xhatch thermal width" should be NOT ticked.

Under "Clearances" tab:
- Thru pin -> Thermal/ant -> Oversize value: 0.1
- SMD pin -> Thermal/ant -> Oversize value: 0.1
- Via -> Thermal/ant -> Oversize value: 0.1
- Line/cline -> (DRC) -> 0.0
- Text -> (DRC) -> 0.0
- Shape/rect -> (DRC) -> 0.0
