## Meta
* Project: python nose
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: Bug Identified
* Brief description (This can change as you progress) :

Python's nose library does not change behavior when the filetype of a loaded python file is a fifo.


## Updates


### Week 3

**Current Stage: Bug Identified**

Bug discovered when changing file types in an fstat call with rreplay. This could indicate a race condition in the loading of files or could cause the program to hang.
