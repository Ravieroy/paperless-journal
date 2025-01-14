???+ Note
	Downloaded the latest Julia version (vx.y.z), however, the Jupyter notebooks uses Julia a.b.c

### Run the following to get the list of kernels and the paths to them
```julia
jupyter kernelspec list
```

Output
```
Available kernels:
  julia-1.9    /home/raviroy/.local/share/jupyter/kernels/julia-1.9
  python3      /home/raviroy/anaconda3/share/jupyter/kernels/python3
```

### Uninstall the old kernels
```julia
jupyter kernelspec uninstall unwanted-kernel
```

### Install `IJulia`
```julia
using Pkg
Pkg.add("IJulia")
```

### Build `IJulia`
```julia
] build IJulia
```
