# Build tools for OpenFOAM on Isambard

These scripts and instructions provide the tools necessary to build a new version of OpenFOAM on the Isambard 2 XCI partition with GCC
First, clone this repository to access the build script:

```shell script
git clone https://github.com/gw4-isambard/openfoam
```
Then submit the build script to the job queue:
```shell script
cd openfoam
qsub build_openfoam
```

The installation directory can be specified by changing the ```$SOFTWARE_HOME``` variable in the ```build_openfoam``` script.

To activate the OpenFOAM installation, either load the newly created OpenFOAM module and run the new ```foamActivate``` script:
``` shell script
THIS DOESN'T WORK - source manually
module use ~/software/xci/modules/gcc-9.3.0
module load openfoam/v2306
foamActivate
```
or do it manually:
``` shell script
source ~/software/xci/packages/gcc-9.3.0/openfoam/v2306/OpenFOAM-v2306/etc/bashrc
```

Example submission scripts for OpenFOAM can be found on the Isambard documentation: https://gw4-isambard.github.io/docs/applications/openfoam.html
