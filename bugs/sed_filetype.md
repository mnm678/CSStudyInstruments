## Meta
* Project: sed
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: Bug Identified
* Brief description (This can change as you progress) :

The sed command does not error when the filetype is changed to a directory in crash simulator.


## Updates


### Week 1

**Current Stage: Bug Identified**

Bug discovered when changing file types in an fstat call with rreplay. After discovering it, I found that the tool does not work for directories, and usually displays an error. I will investigate why the error does not appear when the fstat is changed. It is possibly checked earlier, but not checking again could allow for a race condition.
