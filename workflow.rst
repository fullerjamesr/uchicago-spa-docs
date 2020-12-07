Recommended cryo-EM SPA project workflow
========================================

.. image:: img/CryoEMAcademicWorkflow.*

We recommend that single-particle cryo-EM projects on novel targets proceed through a 3-step workflow.

Before commencing, however, please do make every effort to ensure that the sample is **monodisperse** and **reasonably pure** in bulk solution, and in a buffer that is optmized for its stable folding.

====

The first *screening* stage occurs simply by examining grids by eye. The goal of this stage is to find the sample concentration and (potentially) buffer conditions which result in:

* Particles that are roughly the expected size (as opposed to large aggregates or complexes that have been reduced to their components)
* Fields of those particles which are as dense as possible *while remaining obviously separable and thus pickable*
* Aggregation may be inevitable, but the balance between aggregates and single particles should be optimized to maximize the number of useful intact particles per field of view

In almost all cases, the most useful variable to screen first is sample concentration. Ice thickness (blot time) can be tweaked slightly over the course of the entire workflow.

Common issues arising in this stage are aggregation or particles that adhere to the support surface without entering the holes. These can be addressed by higher (force particles into the holes) or lower (reduce aggregation) sample concentrations, exploring the use of detergents added immediately before blotting as surfactants, or exploring the use of `thin continuous support films <continuoussupportsurfaces>`.

====

Having arrived at a set of conditions that produce particles that are single, dense, but obvious to pick, the next stage involves acquisition of a pilot dataset consisting of approx. 200 to 300 micrographs. Processing this data to 2D class averages or (even better) 3D models provides important information:

* Are the particles visible to the eye capable of being aligned and averaged?
* Do those 2D averages resemble expectations for the target particle?
* Is there a sufficient spread of particle orientation ("views") to allow for 3D reconstruction?

The most common issue at this stage is the final bullet above: problematic preferential orientation. This can often be addressed by detergents or switching to continuous support surfaces.

====

The final stage is the collection of the full dataset (generally 3k-4k micrographs over a 24 hour time slot) on a Krios microscope. For this stage, we recommend submitting ~ 4 samples. These should be duplicates at a macro level -- you should know enough about your sample and how it freezes at this point so that you would be happy to collect from any of them! -- but can also encompass a small gradient in blot times to further optimize ice thickness.