# Furnace Controller V2

Open `Furnace_Controller.kicad_pro` as the project entry point.

The root schematic is the system sheet. Functional sheets are named by their
role (power conversion, communications, supervision, I/O, Ethernet, and relay
drivers). Repeated relay and 3.3 V regulator channels intentionally share a
single child-sheet source.

Project-local TI symbols and footprints are declared in `sym-lib-table` and
`fp-lib-table`; their source files live in `../libraries/Symbols/`. Child
schematics live in `sheets/`; generated Gerbers and assembly outputs live in
`fabrication/`, while PDFs and 3D exports live in `documentation/`.
