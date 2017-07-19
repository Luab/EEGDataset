# EEGDataset
Small dataset of Innopolis University, created during Summer Internship 2017. Could be updating (or not)

### Recording setup
  
  * Device: OpenBCI
  * Placement location: FP1 as first channel, FP2 as a second one. 10-20 international used.
  * Reference: right earlobe A1 position
  * BIAS: left earlobe A2 position
  * Sampling frequency: 250Hz
  * Filtering: No hardware filter was applied, so we highly recommend to use at least 50Hz notch filter to remove enviromental noise. 


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
The folder itself contains the same data stripped from unsued channel data, timestamp and AUX OpenBCI data (such as gyroscope).
Feel free to use this auxilary data as well. 

### Task description

 1. Alpha waves: We intended to capture Alpha waves to achive our task of user authorization. Subjects were asked to sit comfortably and relax. Short time after they relaxed, recording started. Duration of each record is 5 minutes
 2. Counting closed, counting open: Subjects were asked to sit comfortably. After a short period of relaxation they pressed the recording button and second after started to count from 1 to 10. Interval between each number is roughly equal to 1 second. After counting ended they waited another second and recording was stopped. There are two versions of this task, one is perfomed with opened eyes and another with closed. The experiment procedure was the same for both.
 3. Random task: Subjects were asked to think some repeatable task for themselves i.e. imagining his favourite colour, singing his favourite song or play melody of they favourite music in the head or imagine themselves into some place. Task should be performed for at least 10 seconds.
