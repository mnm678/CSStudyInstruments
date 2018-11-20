## Meta
* Project: sed
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: Bug Identified
* Brief description (This can change as you progress) :

The sed command does not error when the filetype is changed to a FIFO in crash simulator.


## Updates


### Week 1

**Current Stage: Bug Identified**

Bug discovered when changing file types in an fstat call with rreplay. The program seems to check for character devices and behave differently, but it does not check for a FIFO


### Week 2

**Source of Bug Diagnosed:**

I looked in the sed source code for when it checks for the file type. It only checks for symlinks. The documentation seems to support using sed on a fifo or character device so this appears to be expected behavior.
