ITKIOWrapper.jl provides wrapper functions in Julia from the InsightToolkit Image Registration functions.

Usage::

```
using ITKIOWrapper
```

Loading Spatial meta data from an image file path:

```
spatialMeta = ITKIOWrapper.loadSpatialMetaData("filepath")

spatialMeta.origin

spatialMeta.spacing

spatialMeta.size
```

Loading Voxel data from an image file path and spatial meta data

```
voxelData = ITKIOWrapper.loadVoxelData("filepath",spatialMeta)
voxelData.dat
```



