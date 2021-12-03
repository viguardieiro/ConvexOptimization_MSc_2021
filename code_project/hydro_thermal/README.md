# Hydro-thermal power system planning

The Brazilian interconnected power system has four regions, SE, S, N and NE, denoted by 0,1,2,3 for simiplicity. In each region, there are one integrated reserviour and several thermal plants to provide energy. Energy exchange is allowed between regions and an additional transshipment station. If demand can not be satisfied, a deficit cost will be incur.

The objective is to minimize the total cost over the designing period meanwhile meeting energy requirements and feasibility constraints.

The available implementation is deterministic (we know the values of all the variables at each stage).

Data available at: https://github.com/lingquant/msppy/tree/master/doc/source/examples/hydro_thermal

## Notation

$v_{it}$: stored energy in subsystem (reservior) $i$ at the beginning of stage $t$  
$a_{it}$: energy inflow in subsystem $i$ during stage $t$   
$q_{it}$: turbined energy (hydro generation) in subsystem $i$ during stage $t$  
$s_{it}$: modelilled energy in subsystem $i$ during stage $t$  
$g_{kt}$: thermal generation at stage $t$ of thermal plants $k$ in each subsystem $i$ during stage $t$  
$\textrm{ex}_{i\rightarrow j,t}$: energy exchange from subsystem $i$ to subsystem $j$  
$\textrm{ex}_{j\rightarrow i,t}$: energy exchange from subsystem $j$ to subsystem $i$  
$\textrm{df}_{ijt}$: deficit account for subsystem $i$ in subsystem $j$ 

## Results

![Histogram - Generation cost in different scenarios](https://github.com/viguardieiro/ConvexOptimization_MSc_2021/tree/main/code_project/hydro_thermal/image/hist_generation.svg?raw=true)

![Plot - Generation cost in consecutive scenarios](https://github.com/viguardieiro/ConvexOptimization_MSc_2021/tree/main/code_project/hydro_thermal/image/plot_generation.svg?raw=true)