## Meta
* Project: perl
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: Bug Identified
* Brief description (This can change as you progress) :

The perl command does not error when the filetype is changed to a FCHR in crash simulator.


## Updates


### Week 2

**Current Stage: Bug Identified**

Bug discovered when changing file types in an fstat call with rreplay. When the input file is changed to a character device or directory the behavior does not change.
