
# Illustrative style guide

A pictured guide for creating @dsgoodsell`s iconic illustrative style in #molstar.

We will use the Golgi Casein Kinase (PDB 5yh2) #motm as an example https://pdb101.rcsb.org/motm/265.

View the final state online https://molstar.org/viewer/?snapshot-url=https://molstar.org/viewer-docs/tips/movie-export/5YH2-illustrative.molx&snapshot-url-type=molx

![5YH2](5YH2.png)


# Load PDB and reset style

1. Load PDB 5YH2 using the Download Structure action in the top left
2. Clear all visuals by selecting the "Empty" preset in the Components panel
3. Add a spacefill representation for everything

![Load structure](load-structure.png)

![Empty preset](empty-preset.png)

![Add spacefill](add-spacefill.png)

![UI spacefill](ui-spacefill.png)


# Adjust selection

4. Activate selection mode; pick "Chain" granularity; click on chains to be removed
5. "Subtract" your selection from the "All" entry in the Components panel

![Select chains](select-chains.png)

![Remove selected](remove-selected.png)

![UI removed](ui-removed.png)


# Adjust coloring

6. Select the "Illustrative" color theme for our "Spacefill" representation
7. Change the "Asym Id" option to "Label"
8. Enable theme legend; drill down to color list; change colors for our chains

![Color illustrative](color-illustrative.png)

![Illustrative label](illustrative-label.png)

![Adjust color](adjust-color.png)

![UI adjusted](ui-adjusted.png)


# Adjust lighting

9. Enable occlusion and outline in the Settings menu; tweak occlusion bias and outline threshold
10. Enable "Ignore Light" option for our "Spacefill" representation

Congratulations, you made it through a lot of tedious (but powerful) UI actions. Enjoy and share.

![Outline occlusion](outline-occlusion.png)

![Ignore light](ignore-light.png)

![UI final](ui-final.png)
