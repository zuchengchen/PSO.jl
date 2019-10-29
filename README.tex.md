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
$$
    v_j^{(i)}[k+1] = w * v_j^{(i)}[k] + c_1 * r_1,j * (p_j^{(i)}[k] - x_j^{(i)}[k]) + c_2 * r_2,j * (g_j^{(i)}[k] - x_j^{(i)}[k])
$$

* position update
$$
    x_j^{(i)}[k+1] = x_j^{(i)}[k] + v_j^{(i)}[k+1]
$$

* $\bar{x}^{(i)}[k]$: Position of $i$th particle in $k$th iteration

$$
    \bar{x}^{(i)}[k] = (x_0^{(i)}[k], x_1^{(i)}[k], ..., x_D^{(i)}[k])
$$

* $\bar{v}^{(i)}[k]$: velocity of $i$th particle in $k$th iteration

$$
    \bar{v}^{(i)}[k] = (v_0^{(i)}[k], v_1^{(i)}[k], ..., v_D^{(i)}[k])
$$
