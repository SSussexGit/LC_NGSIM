# LC_NGSIM
lane change trajectories extracted from NGSIM
**To use this data, please cite this paper, thank you!**
```
@INPROCEEDINGS{Dong2017_3,
   Author = {C. Dong, Y. Zhang and J. Dolan},
   Title = {Lane-Change Social Behavioral Generator for Autonomous Driving Car by Non-parametric Regression in Reproducing Kernel Hilbert Space.},
   Booktitle = {Proc. of The International Conference on Intelligent Robots and Systems (IROS)},
   Year = {2017},
   organization={IEEE}
}
```
## Source Code.
For source code, click [here](https://github.com/donnydcy/LC_NGSIM/blob/master/src/README.md)

## Data description
### nlc_data_5zones.mat 
- nlc_data: *cell, contains 870 sequences of none-lane-change scenarios.*
  * veh_s: *subjcet vehicle*
    + **x**: *Lateral position (m)*
    + **y**: *Longitudinal position (m)*
    + **len**: *Vehicle length (m)*
    + **wid**: *Vehicle width (m)*
    + **v**: *Vehicle speed (m/s)*
    + **a**: *Vehicle acceleration (m/s^2)*
  * veh_f: *front vehicle in current lane*
  * veh_r: *rear vehicle in current lane*
  * veh_ft: *front vehicle in target lane*
  * veh_rt: *rear vehicle in target lane*
  * veh_st: *overlap vehicle in target lane*         
### lc_data_20s_withpoints.mat
- lc_data: *Same structure as nlc_data*
- points: *array, n row, 2 column, [start, end]*