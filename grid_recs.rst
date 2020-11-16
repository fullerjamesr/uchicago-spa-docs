What grids should I buy?
========================

Lab starter pack
----------------

.. admonition::
   The basics
   
   * Quantifoil 1.2/1.3 300 Cu mesh (carbon foil on copper mesh) for dirt-cheap initial screening by eye (EMS catalog number Q350CR1.3 for a 50 pack)
   * C-flat 1.2/1.3 300 Au mesh (carbon foil on gold mesh) for routine work, optimization, data collection (EMS catalog number CF313-50-Au for a 50 pack)

.. admonition::
   If you're feeling lucky

   UltrAuFoil 1.2/1.3 300 mesh (gold foil on gold mesh) for structures where beam-induced motion is the remaining limitation to resolution (EMS catalog number Q350AR13A for a 50 pack)

.. admonition::
   For samples that need a continuous support surface

   Quantifoil 1.2/1.3 300 Au mesh with Ultrathin carbon (2 nm amorphous carbon on carbon foil on gold mesh) (EMS catalog number Q350AR1.3-2nm for a 50 pack)

See the rest of this page for more detailed information and opinions.

Mesh and hole sizes
-------------------

.. figure:: img/grid_geom.*
   
   Source: Protochips

**Mesh** refers to how large the grid **squares** are. Common sizes are 200, 300, and 400. In this case *lower numbers* are *bigger squares*.

**Hole diameter** and **hole spacing** are given in microns. Note that hole spacing refers to the edge-to-edge distance between holes, not center-to-center. The true size of the holes is usually pretty consistent within a grid but routinely varies by 5-15% from the value given on the label.

Grid specs are usually given in the form of "diameter/spacing mesh" as in  "1.2/1.3 300".

Mesh size considerations
^^^^^^^^^^^^^^^^^^^^^^^^
Smaller squares arise from a more dense array of the underlying grid support bars. Thus, grids with smaller squares (400 mesh) tend to be more resilient to bending during handling.

However, there are compelling advantages to larger squares (200 or 300 mesh) that arise from the following:

1. Generally, ice thickness tends to differ most dramatically between squares (and fall within a narrow range within a given square).
2. Best practice is to disregard a cracked square entirely during data collection. If the foil surface is cracked or damaged within a square, this usually leads to larger beam-induced specimen movement.
3. Physical stage movement is slow and inaccurate, and thus wastes collection time.

For collection speed, larger squares contain more holes, which means fewer stage movements are needed to collect from the same number holes (assuming image shift-based data collection). Furthermore, (1) and (2) above mean that square selection is a binary choice, and so to collect the same number of holes, you need to get lucky (the coincidence of no-cracks and good-ice-thickness) on fewer grid squares if they are larger.

.. tip::
   James recommends 300 mesh

Hole size/spacing considerations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Most SPA is done on either 1.2/1.3 or 2/1 holes. Your ideal hole geometry depends (or dictates) on the data collection strategy:

* Larger holes (2 micron) can allow for multiple exposures to be taken of non-overlapping regions of the same hole.
* Smaller holes (1.2 micron) can pack more holes into the same surface area, but realistically only allow for a single exposure in each hole.

.. tip::
   So who wins for data collection speed? **In our hands, it's virtually a wash.** We have seen both 1.2/1.3 with 1 exposure per hole and 2/1 with multiple shots per hole reach up to ~ 280 exposures per hour.

**New, October 2020**: `Recent work on specimen movement as a function of hole size <https://science.sciencemag.org/content/370/6513/223>`_ showed that smaller holes minimize movement (see Figure 1B and C). Quantifoil now has 0.6 micron holes sizes regularly available, maybe we should be switching to that!

.. tip::
   James recommends 1.2/1.3 foils

Materials
---------
Grid support
^^^^^^^^^^^^

.. topic:: Copper

   Historically, the grid support (grid bars, etc) used for cryo-EM SPA have been made from copper. Copper is strong, conducts electrons, and is relatively inexpensive.

   However, copper and amorphous carbon have mismatched thermal expansion coefficients that build strain in the support surface during freezing. This strain is released during exposure to the electron beam.

.. topic:: Gold

   The gold::carbon thermal expansion mismatch is about a third the magnitude.

Foil
^^^^

.. topic:: Carbon

   Historically, holey amorphous carbon has been used as the support surface for cryo-EM SPA. It is chemically inert and trivial to make hydrophilic by glow discharge.

   However, amorphous carbon films are only semiconductors (and in practice, their resistivity varies batch-to-batch), and so charging effects during exposure can add to beam-induced movement. Once again...

.. topic:: Gold
   
   Gold foils have orders of magnitude smaller electrical resistivity.
   
   The downside of gold foils is that they take somewhat less readily to being made hydrophilic. They often need longer glow discharge exposure time, which increases the risk of thinning and damage to the foil.
   
All-gold grids
^^^^^^^^^^^^^^

The above observations lead to the introduction of all-gold grids, sold under the name **UltrAuFoil** by Quantifoil and under the name **Au-Flat** by Protochips/C-flat.

Grids where both the foil and suports are made of gold have the benefit of having uniform low resistivity, and uniform (matched) thermal expansion. Because gold is a more malleable material, these grids are somewhat more easy to bend during handling, but that is at least partially offset by being somewhat less prone to being cracked when bent.

----

This is an excellent reference testing the properties of carbon/copper versus gold: https://www.sciencedirect.com/science/article/pii/S1047847715301039

Brands
------
There are two major manufacturers of holey TEM grids:

* `Quantifoil <https://www.quantifoil.com>`_
* `Protochips (C-flat) <https://www.protochips.com/products/c-flat/>`_.

There are non-trivial differences in how each company manufactures the holey surface.

Quantifoil tend to be cheaper, but:

* The holey surface deviates more from perfect flatness. While this is probably not a big deal when you're collecting a large dataset from any single grid, it can make grid-to-grid reproducibility less robust.
* There have been occasional reports of batches with residual compounds on the grid surface that behave poorly (in terms of hydrophilization or interactions with sample). *Such reports are difficult to verify and may be apocryphal, but occur often enough to be worth mentioning*.

James' completely arbitrary recommendations
-------------------------------------------
My favorite grids are the C-flat 1.2/1.3 300mesh Au grids. Having gold support bars eliminates the majority of the excess beam-induced movement seen in copper grids, while a carbon surface is reliably easy to make hydrophilic. 300 mesh is a nice compromise between strength (gold is more flimsy vs. copper, so gold 200 mesh can be quite bendy) and holes per square.

*However, in cases where you have a very good sample and are thus limited by beam-induced movement*, the entirely-gold grids (either UltrAuFoil or Au-Flat, which are also available as 1.2/1.3 300 mesh) can work quite well!
