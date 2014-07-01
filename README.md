Playground.jl
=============

A package for managing julia sandboxes like python's virtualenv.

### Usage ###
#### Create ####
To create a new playground using your existing julia install.
```shell
playground /path/of/new/playground create
```
To create a new playground with a specific pre-built julia binary.
```shell
playground /path/of/new/playground create --julia /path/to/julia/executable
```
To create a new playground with a specific version of julia.
```shell
playground /path/of/new/playground create --julia v0.1
```
To create a new playground with a specific git revision of julia.
```shell
playground /path/of/new/playground create --julia 9effcb3
```
NOTES:
* The last two examples involve rebuilding julia from source and will take a long time.
* When creating a new playground you can pass a `--clean` which will delete any existing files in the playground directory if it is an existing playground.

#### Activate ####
To activate a given playground simply run.
```shell
playground /path/to/your/playground activate
```

#### TODOs ####
* Tests
* Logging
* travis config
* untested on non-linux platforms!
* Add to METADATA.jl