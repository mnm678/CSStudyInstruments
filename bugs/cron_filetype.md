## Meta
* Project: crontab
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: Bug Identified
* Brief description (This can change as you progress) :

The crontab command does not error when the filetype of crontab is changed from a directory to a character device in the stat call.


## Updates


### Week 1

**Current Stage: Bug Identified**

Bug discovered when changing file types in an fstat call with rreplay. Multiple fstat calls do not respond to a change in the st_mode.

### Week 2

I couldn't reproduce this bug with an updated version of crash simulator. I will continue to investigate.
