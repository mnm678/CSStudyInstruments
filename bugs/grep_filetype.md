## Meta
* Project: grep
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: Bug Identified
* Brief description (This can change as you progress) :

The grep command does not error when the filetype is changed to a character device.


## Updates


### Week 1

**Current Stage: Bug Identified**

Bug discovered when changing file types in an fstat call with rreplay. After discovering it, I found that grep seems to hang with a character device as input.
