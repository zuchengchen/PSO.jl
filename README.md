# PSO.jl
Particle swarm optimization written in julia.

[![Stable](https://img.shields.io/badge/docs-stable-blue.svg)](https://bingining.github.io/PSO.jl/stable)
[![Dev](https://img.shields.io/badge/docs-dev-blue.svg)](https://bingining.github.io/PSO.jl/dev)

PSO.jl is the julia implementation of Particle swarm optimization algorithm.

## Installation

```julia
julia> using Pkg;
julia> Pkg.add(PackageSpec(url="https://github.com/bingining/PSO.jl.git"))
```


## Usage

Tutorials can be found at [examples](https://github.com/bingining/PSO.jl/tree/master/examples).

# PSO dynamical equations
* velocity update
<p align="center"><img src="/tex/3a1216884a50c3001ef914328adfde8d.svg?invert_in_darkmode&sanitize=true" align=middle width=590.9243966999999pt height=23.9884194pt/></p>

* position update
<p align="center"><img src="/tex/24c57802b81724c96995c8279eaaebbe.svg?invert_in_darkmode&sanitize=true" align=middle width=227.8413291pt height=23.9884194pt/></p>

* <img src="/tex/dc65f93b783cb4aa34846c23d3f69fb5.svg?invert_in_darkmode&sanitize=true" align=middle width=43.34959529999998pt height=29.190975000000005pt/>: Position of <img src="/tex/77a3b857d53fb44e33b53e4c8b68351a.svg?invert_in_darkmode&sanitize=true" align=middle width=5.663225699999989pt height=21.68300969999999pt/>th particle in <img src="/tex/63bb9849783d01d91403bc9a5fea12a2.svg?invert_in_darkmode&sanitize=true" align=middle width=9.075367949999992pt height=22.831056599999986pt/>th iteration

<p align="center"><img src="/tex/62775c5d5f5ff8743db9fc579b686717.svg?invert_in_darkmode&sanitize=true" align=middle width=243.71783369999997pt height=21.99987075pt/></p>

* <img src="/tex/33cd374b9893a130ab6a666099989c9f.svg?invert_in_darkmode&sanitize=true" align=middle width=42.51245294999999pt height=29.190975000000005pt/>: velocity of <img src="/tex/77a3b857d53fb44e33b53e4c8b68351a.svg?invert_in_darkmode&sanitize=true" align=middle width=5.663225699999989pt height=21.68300969999999pt/>th particle in <img src="/tex/63bb9849783d01d91403bc9a5fea12a2.svg?invert_in_darkmode&sanitize=true" align=middle width=9.075367949999992pt height=22.831056599999986pt/>th iteration

<p align="center"><img src="/tex/8fb144d075ea3b34d6e800ca6e1ee79f.svg?invert_in_darkmode&sanitize=true" align=middle width=240.36925275pt height=21.99987075pt/></p>
