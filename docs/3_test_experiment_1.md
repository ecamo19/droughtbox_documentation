---
title: Dermination of residual water loss from small branches 
---

This protocol describes how to measure g<sub>res</sub> under __constant temperature and relative humidity__ 

# Procedure

## Materials-Equipments

+ Paraffine wax
+ Scale
+ Scanner
+ ImageJ

## Plant material preparation 

+ Collect 1 to 1.5 meters long branches  
+ Cut the end of each branch underwater
+ Rehydrate plants overnight by immersing them in water
+ Cover the branches with black plastic bags and store them dark conditions

## Before starting the measurements

+ Recut a 40 cm long branch (weight should not be larger than 100 grams)
+ Measure the fresh weight of each branch
+ Measure the diameter of the branch at the cut end and at the top of branch 
+ Seal the end of the branch with parafilm
+ Check there is water in the reservoir located inside the box
+ Before placing the branches inside the Box, 
	+ Set the temperature and relative humidity values and wait until these stabilize (You can use this [VPD Calculator](https://cales.arizona.edu/vpdcalc/))
	+ Change the `TareNow` flag (located in the Num Display window) from `false` to `true` 
	
## During the measurements 




## Data Analysis

$$E = \frac{slope(n_w;t)}{LA\ +\ BA }$$


$$g_{res}= \frac{E}{VPD}\ \times 101.6$$
## Code
```python
import pandas
```


