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
0|20|M|Imagining favourite color
1|20|M|Typing on a keyboard
2|19|M|Walking through a well known place
3|22|M|Listening to wind and trees 
4|19|F|Not available
5|18|F|Not available
6|28|M|Singing favourite song
7|17|M|Not available
8|20|M|Singing favourite song
9|19|M|Singing favourite song
10|31|M|Walking through home and picking up known object
11|20|M|Showing magic tricks
12|20|M|Imagining himself an absolute
13|27|F|Taking a shower
14|18|M|Freefalling
15|26|M|Imagining a logo of his company
16|24|F|Singing a song
17|23|F|Being in a familiar place
18	|	21|M|	Riverside of Volga from a bicycle
19	|	18|M	|Being rewarded by medal at school graduation ceremony
20	|17|M|	Riding a bycicle
21	|	18|M|	Playing football
22	|18|M|	Familiar song
23	|18	|M| Interior of a room from sitcom
24	|18|M| Imagining his cat
25	|24|F|	Room in a house
26	|18|M|	Father
27  |18|M	|Typing keyboard in his room
28	|18|M	|Attic with window and sunbeams
29	|	17|M|	Mick Jagger performance
30	|17|M|	Kazan-Arena stadium
31	|19|M	|Solving math tasks
32	|18	|M|Singing by a campfire
33	|	18|M|	Pouring cola from one cuo to another
34	|	18|M|	Password
35	|19	| M| Imagining a class
36	|	18|M|	Professor lecture
37	|18| M|	Walking through house
38|56	| M| Mother
39|	18| M	|Riding a bycicle
40|18 |M|			|Impossible triangle 
41	|	19|	M|Opened doors and saw mountines through them
42	|	17|	M|Sining and playing guitar
43|	17	|F|Getting acceptance from a Innopolis university

### Dataset structure
Our dataset is organized as follows. Folder names are coressponding to the type of activity (or mental task) recorded. 
Inside each folder there is a subfolder named "raw" which contains unprocessed OpenBCI files.
The folder itself contains the same data stripped from unsued channel data, timestamp and AUX OpenBCI data (such as gyroscope).
Feel free to use this auxilary data as well. 

### Task description

 1. Alpha waves: We intended to capture Alpha waves to achive our task of user authorization. Subjects were asked to sit comfortably and relax. Short time after they relaxed, recording started. Duration of each record is 5 minutes
 2. Counting closed, counting open: Subjects were asked to sit comfortably. After a short period of relaxation they pressed the recording button and second after started to count from 1 to 10. Interval between each number is roughly equal to 1 second. After counting ended they waited another second and recording was stopped. There are two versions of this task, one is perfomed with opened eyes and another with closed. The experiment procedure was the same for both.
 3. Random task: Subjects were asked to think some repeatable task for themselves i.e. imagining his favourite colour, singing his favourite song or play melody of they favourite music in the head or imagine themselves into some place. Task should be performed for at least 10 seconds.
