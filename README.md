# EEGDataset
Small dataset of Innopolis University, created during Summer Internship 2017. Could be updating (or not)

### Recording setup
  
  * Device: OpenBCI
  * Placement location: FP1 as first channel, FP2 as a second one. 10-20 international used.
  * Reference: right earlobe A1 position
  * BIAS: left earlobe A2 position
  * Sampling frequency: 250Hz

### Subject info

Number|Age|Gender|Custom mental task|
------|---|------|------------------|
0|20|M|
1|20|M|
2|19|M|Walking through a well known place
3|22|M|
4|19|F|
5|18|F|
6|28|M|Singing favourite song
7|17|M|
8|20|M|Singing favourite song
9|19|M|
10|31|M|Walking through a home and picking up known object


### Dataset structure
Our dataset is organized as follows. Folder names are coressponding to the type of activity (or mental task) recorded. 
Inside each folder there is a subfolder named "raw" which contains unprocessed OpenBCI files. 
