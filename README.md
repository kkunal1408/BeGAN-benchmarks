# BeGAN-benchmarks

This is a anonymous public repository which contains thousands of PDN benchmarks in the form of SPICE circuit netlist files for three different technologies: 

- [SkyWater130 HD](https://github.com/google/skywater-pdk)
- [FreePDK45 with Open Cell Library (NanGate 45nm)](https://github.com/The-OpenROAD-Project/OpenROAD-flow-scripts/tree/master/flow/platforms/nangate45)
- [ASAP7](https://github.com/The-OpenROAD-Project/asap7)

## Contents

- real-circuit-benchmarks: These benchmarks are generated using current maps [OpenROAD flow](https://github.com/The-OpenROAD-Project/OpenROAD-flow-scripts/tree/master/flow/platforms/nangate45) with PDN from the OpenROAD flow (regular) and OpeNPDN (irregular). 
- BeGAN-circuit-benchmarks: These benchmarks current maps are generated using the GANs. The PDNs are generated by both the OpenROAD flow (uniform) and OpeNPDN (non-uniform).

 Each benchmark folder contains the following data:
 - BeGAN_*_current_map.csv.gz (matrix representation of the current values) 
 - BeGAN_*_reg_grid.sp.gz (SPICE netlist files for regular PDN)
 - BeGAN_*_irreg_grid.sp.gz (SPICE netlist files for irregular PDN)
 - BeGAN_*_voltage_map_regular.csv.gz (matrix representation of the IR drop across the chip for regular PDN)
 - BeGAN_*_voltage_map_irregular.csv.gz (matrix representation of the IR drop across the chip for irregular PDN)
 
 
 Each benchmark folder also contains image representation for the above data and histogram representation for the following:
 - BeGAN_*_voltage_map_regular_hist.png (per-PDN node IR drop distributions for regular PDN)
 - BeGAN_*_voltage_map_irregular_hist.png (per-PDN node IR drop distributions for irregular PDN)
 - BeGAN_*_voltage_map_regular_cdf.png (per-PDN node cumulative IR drop distributions for regular PDN)
 - BeGAN_*_voltage_map_irregular_cdf.png (per-PDN node cumulative IR drop distributions for irregular PDN)

## Gallery

Sample images from both real circuit and BeGAN benchmarks displayed below for
45nm technology as an example.

### Real circuit current maps
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/aes_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/ibex_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/jpeg_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/bp_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/bp_fe_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/bp_be_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/bp_multi_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/swerv_current_map.png" width="22%"></img> 

### BeGAN benchmark current maps
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_001_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_002_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_004_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_005_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_008_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_994_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_010_current_map.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_024_current_map.png" width="22%"></img> 


### Real circuit IR drop heatmaps
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/aes_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/ibex_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/jpeg_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/bp_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/bp_fe_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/bp_be_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/bp_multi_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/real-circuit-benchmarks/nangate45/images/swerv_voltage_map_regular.png" width="22%"></img> 

### BeGAN benchmark IR drop heatmaps
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_001_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_002_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_004_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_005_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_008_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_994_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_019_voltage_map_regular.png" width="22%"></img> 
<img
src="https://github.com/PDN-BeGAN/BeGAN-benchmarks/blob/master/BeGAN-circuit-benchmarks/nangate45/images/BeGAN_024_voltage_map_regular.png" width="22%"></img> 



## Benchmark description
We use a SPICE format for releasing out benchmarks. An example is listed below
```
R645 n1_108000_179200_1 n1_102600_179200_1 0.14
R646 n1_113400_179200_1 n1_113400_179200_3 4.23
I7 n1_113400_179200_1 0 4.24901e-08
V0 n1_81000_106230_7 0 1.1
```

The generic convention is: `<electric component> <node1> <node2> <value>`

The node is defined using the following convention: `<netname>_<x-cordinate>_<y-cordinate>_<layer-idx>`
In the above example R645 is via since they share the same x and y coordinate but the layer changes. 

## Benchmark examples summary

The table below summarizes the components for randomly sampled BeGAN benchmark
for NanGate 45nm technology.

| BeGAN id  | #nodes                        | #resistors | #voltage sources  | #current sources  |
|-----------|-------------------------------|------------|-------------------|-------------------|
| 1         | 18409                         | 19903      | 4                 | 15750             |
| 2         | 50924                         | 55332      | 9                 | 43472             |
| 3         | 455112                        | 493695     | 64                | 391220            |
| 4         | 112546                        | 122641     | 12                | 95934             |
| 5         | 178555                        | 193018     | 24                | 153738            |
| 6         | 179730                        | 195360     | 24                | 153738            |
| 7         | 82389                         | 89254      | 12                | 70738             |
