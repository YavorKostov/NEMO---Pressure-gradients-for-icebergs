The pre-existing iceberg dynamics code in NEMO parameterizes ocean drag as a function of the vertically averaged ocean velocity components.

A new version of the code is developed here, whereby the ocean velocity at each depth level is used to compute a drag on the iceberg keel. The ocean drag is then vertically averaged over the depth of the keel.

If you replace icbdyn.F90 with icbdyn.F90_OceanDrag_VerticalProfile provided here, you will apply the updated ocean drag.

This development merits its own branch separate from the introduction of updated pressure gradients in the iceberg dynamics.