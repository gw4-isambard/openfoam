# Build tools for OpenFOAM on Isambard

These scripts and instructions provide the tools necessary to build a new version of OpenFOAM on the Isambard 2 XCI partition with GCC
First, clone this repository to access the build script:

```shell script
git clone https://github.com/gw4-isambard/openfoam
```
Then run the build script:
```shell script
cd openfoam
./build_openfoam
```

The installation directory ad target programming environmet can be changed within the script.

To activate the OpenFOAM installation, either load the newly created OpenFOAM module and run the new ```foamActivate``` script:
``` shell script
module use ~/software/modules/cray
module load openfoam/v2312
source foamActivate
```

Example submission scripts for OpenFOAM can be found on the Isambard documentation: https://gw4-isambard.github.io/docs/applications/openfoam.html
