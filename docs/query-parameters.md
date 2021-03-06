
# Query Parameters

## Parameters

### `hide-controls`
This will hide the UI panels on all sides. If `1` the controls are hidden. For all other values the controls are shown. By default the controls are shown. Clicking on the wrench icon in the top right of the canvas will toggle the visibility of the controls.

    hide-controls=1
    
### `collapse-left-panel`
This will collapse the left UI panel to a vertical icon bar. If `1` the left panel is collapsed. For all other values the left panel is fully shown. By default the left panel is fully are shown. Clicking on an icon in the vertical icon bar will toggle between the collapsed and fully shown state.

    collapse-left-panel=1

### `pdb-provider`
Where to load PDB entries from. Allowed values are `pdbe` and `rcsb`. Defaults to `pdbe`. From Europe, `pdbe` generally offers faster PDB downloads. From the Americas, `rcsb` is faster.

    pdb-provider=pdbe

### `emdb-provider`
Where to load EMDB entries from. Allowed values are `pdbe` and `rcsb`. Defaults to `pdbe`. From Europe, `pdbe` generally offers faster EMDB downloads. From the Americas, `rcsb` is faster.

    emdb-provider=pdbe

### `snapshot-url`
URL pointing to a molstar snapshot. Use `snapshot-url-type` to define the type.

    snapshot-url=https%3A%2F%2Fmolstar.org%2Fdemos%2Fstates%2Fbtub.molx

### `snapshot-url-type`
Allowed values are `molj` and `molx`.  Defaults to `molj`.

    snapshot-url-type=molj

### `structure-url`
URL pointing to a structure file.

    structure-url=https://files.rcsb.org/download/6Z1W.cif

### `structure-url-format`
Allowed values `mmcif`, `pdb`, `gro`, `sdf`, `mol2`, ...

    structure-url-format=mmcif

### `structure-url-is-binary`
If `1` binary, otherwise not binary.

    structure-url-is-binary=1

### `pdb`

    pdb=3pqr

### `pdb-dev`

    pdb-dev=PDBDEV_00000030

### `emdb`

    emdb=EMD-23149

### `debug-mode`
If `1` enabled, otherwise not. This will print debug info to the browser console and performs (expensive) runtime checks.

    debug-mode=1

## Examples
Load a molx snapshot from an URL

    https://molstar.org/viewer/?snapshot-url=https%3A%2F%2Fmolstar.org%2Fdemos%2Fstates%2Fbtub.molx&snapshot-url-type=molx

Load a mmCIF file from an URL

    https://molstar.org/viewer/?structure-url=https://files.rcsb.org/download/6Z1W.cif&structure-url-format=mmcif

Load PDB entry

    https://molstar.org/viewer/?pdb=3pqr

Load PDB-Dev entry

    https://molstar.org/viewer/?pdb-dev=PDBDEV_00000030

Load EMDB entry

    https://molstar.org/viewer/?emdb=EMD-23149
