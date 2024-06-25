# Singularity_GISTIC
[![Apptainer-deploy](https://github.com/panxiaoguang/Singularity_GISTIC/actions/workflows/build.yml/badge.svg)](https://github.com/panxiaoguang/Singularity_GISTIC/actions/workflows/build.yml)
 Build Gistic2 apptainer image using Github Action

## Usage

you can also use `Gistic2.def` from this repo to build your gistic2 image locally using singularity.

```bash

singularity build -f gistic2.sif Gistic2.def

``` 

## how to run

first download the image from release page or build it locally using above command.

then run the image using singularity.

```bash
singularity exec Gistic2.sif gistic2 --help
```

## Note: 
If you meet a situation of losing some dependencies, please use `--cleanenv` to exec singularity, like:

```bash
singularity exec --cleanenv Gistic2.sif gistic2 --help
```

