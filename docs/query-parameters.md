
# Query Parameters

The Mol* Viewer supports a number of URL [parameters](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_URL#parameters) to load structures and change viewer options.

## Parameters

### `hide-controls`
This will hide the UI panels on all sides. If `1` the controls are hidden. For all other values the controls are shown. By default the controls are shown. Clicking on the wrench icon in the top right of the canvas will toggle the visibility of the controls.

    hide-controls=1

### `collapse-left-panel`
This will collapse the left UI panel to a vertical icon bar. If `1` the left panel is collapsed. For all other values the left panel is fully shown. By default the left panel is fully are shown. Clicking on an icon in the vertical icon bar will toggle between the collapsed and fully shown state.

    collapse-left-panel=1

### `pdb-provider`
Where to load PDB entries from. Allowed values are `pdbe`, `pdbj` and `rcsb`. Defaults to `pdbe`. From Europe, `pdbe` generally offers faster PDB downloads. From Asia-Pacific, `pdbj` is usually faster. From the Americas, `rcsb` is usually faster.

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
Load one or more (comma separated) [PDB](https://www.wwpdb.org/) entries.

    pdb=3pqr

### `pdb-dev`
Load one or more (comma separated) [PDB-Dev](https://pdb-dev.wwpdb.org/) entries.

    pdb-dev=PDBDEV_00000030

### `emdb`
Load one or more (comma separated) [EMDB](https://www.ebi.ac.uk/emdb/) entries.

    emdb=EMD-23149

### `afdb`
Load one or more (comma separated) [AlphaFold DB](https://alphafold.ebi.ac.uk/) entries.

    afdb=Q8W3K0

### `model-archive`
Load one or more (comma separated) [Model Archive](https://www.modelarchive.org/) entries.

    model-archive=ma-bak-cepc-0003

### `debug-mode`
If `1` enabled, otherwise not. This will print debug info to the browser console and performs (expensive) runtime checks.

    debug-mode=1

### `pixel-scale`
How many rendered pixels correspond to displayed pixels. Defaults to 1. Set to < 1 for a more blurry, pixelated but faster rendered image. Set to > 1 for a sharper, less pixelated but slower rendered image.

    pixel-scale=1

### `disable-wboit`
If `1`, WBOIT is disabled, otherwise it is enabled. WBOIT stands for 'weighted blended order-independent transparency' [[McGuire & Bavoil, JCGT 2013](https://jcgt.org/published/0002/02/09/)]. It allows more acurate rendering of overlapping transparent objects at the expense of some speed.

    disable-wboit=1

## Examples
Load a molx snapshot from an [URL](https://molstar.org/viewer/?snapshot-url=https%3A%2F%2Fmolstar.org%2Fdemos%2Fstates%2Fbtub.molx&snapshot-url-type=molx)

    https://molstar.org/viewer/?snapshot-url=https%3A%2F%2Fmolstar.org%2Fdemos%2Fstates%2Fbtub.molx&snapshot-url-type=molx

Load a mmCIF file from an [URL](https://molstar.org/viewer/?structure-url=https://files.rcsb.org/download/6Z1W.cif&structure-url-format=mmcif)

    https://molstar.org/viewer/?structure-url=https://files.rcsb.org/download/6Z1W.cif&structure-url-format=mmcif

Load PDB entry [3PQR](https://molstar.org/viewer/?pdb=3pqr)

    https://molstar.org/viewer/?pdb=3pqr

Load PDB-Dev entry [PDBDEV_00000030](https://molstar.org/viewer/?pdb-dev=PDBDEV_00000030)

    https://molstar.org/viewer/?pdb-dev=PDBDEV_00000030

Load EMDB entry [EMD-23149](https://molstar.org/viewer/?emdb=EMD-23149)

    https://molstar.org/viewer/?emdb=EMD-23149

Load AlphaFold DB entry for UniProt AC [Q8W3K0](https://molstar.org/viewer/?afdb=Q8W3K0)

    https://molstar.org/viewer/?afdb=Q8W3K0

Load Model Archive entry [ma-bak-cepc-0003](https://molstar.org/viewer/?model-archive=ma-bak-cepc-0003)

    https://molstar.org/viewer/?model-archive=ma-bak-cepc-0003
