# gadal IEEE123 version

Changes to default opendss solution:

1. Changing load model 1 to load model 8
2. Add load and pv data.
3. Create corresponding OEDI entry


The data should be able to be run in a gadal feeder with state estimator and optimal power flow.

# Directory structure and usage

## Structure

snapshot folder is self-contained i.e. the snapshot/master.dss can be run without any other dependency. QSTS has a dependency on the profiles folder.


## Running a snapshot

One can run the snapshot by running the snapshot/master.dss file.

## Running QSTS

One can run the QSTS by running the qsts/master.dss file. The user is recommended to make any modifications to the profiles in-place i.e. modify the profile shapes in the appropriately named files. It is also possible to make changes any way the user wants but appropriate changes need to be made to the qsts/*.dss files as needed.

## Notes on load model

The snapshot/IEEE123Loads.dss and qsts/IEEE123Loads.dss both have ZIP loads i.e. model=8. This allows the load to vary as a function of voltage.
