### Time series plots

The naming format of these images are `{DWave-device-name}_{N}_results_indicator{I}_AT{AT}_MCprob_{prob}_MA.pdf`

- DWave-device-name is the chip ID, for example `DW_2000Q_LANL` or `DW_2000Q_6`
- N is the size of the all-to-all minor embedding for the problem
- I denote the type of indicator that was used (this is either 1, 2, or 3). 
- AT is the annealing time
- MA is either `no_averages` or `moving_average_` followed by the moving average window. 

Typically these files are simply the raw energies (no unembedding algorithm has been applied). However, some plots are also preceded by `unembedded_` which indicates that the energies are from majority vote unembedded samples. 

Finally, if there was a non-standard modification of the DWave settings, it will be noted after the annealing time. For example `pause0.75` denotes a symmetric pause at an anneal fraction of `s=0.75` was applied during forward annealing.  
