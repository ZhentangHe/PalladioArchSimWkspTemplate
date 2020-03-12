# Palladio Architecture Simulation Workspace Template
This is the workspace template for Palladio Architecture Simulation in Eclipse Che.

## About the devfile
A devfile is a file that describes and define a development environment. 

This `devfile.yaml` includes two projects and one component. NOTE that only the one named `PalladioSimulation` is needed for this workspace. The other one is for test only and contains only the data for the simulation under its path `/PalladioRunExperiment`.

The one component here is a docker container and the repository is [here](https://hub.docker.com/r/palladiosimulator/palladio-experimentautomation).

See more about devfile in [official documentation](https://www.eclipse.org/che/docs/che-7/configuring-a-workspace-using-a-devfile/).

## Usage
There are two ways to use this template. 

You can simply import the `devfile.yaml` in this repository while creating a new workspace in Eclipse Che or use the link 
```
http(s)://che-host:che-port/f?url=https://raw.githubusercontent.com/ZhentangHe/PalladioArchSimWkspTemplate/master/devfile.yaml
``` 
to create a workspace factory. 

Or you can customize your own devfile/plugin registry by adding these two files `devfile.yaml` and `meta.yaml`. The example is given in this [repository](https://github.com/ZhentangHe/che-devfile-registry/tree/palladiodev).
