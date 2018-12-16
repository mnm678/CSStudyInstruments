## Meta
* Project: python nose
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: Bug Fix Submitted to Project
* Brief description (This can change as you progress) :

Python's nose library does not change behavior when the filetype of a loaded python file is a fifo.


## Updates


### Week 3

**Current Stage: Bug Identified**

Bug discovered when changing file types in an fstat call with rreplay. This could indicate a race condition in the loading of files or could cause the program to hang.

### Week 4

**Current Stage: Source of Bug Diagnosed**

The library checks for some irregular file types, but not all of them.

### Week 5

**Current Stage: Bug Fix Submitted to Project**

I changed the checks to look for any irregular file type. The pr was submitted here: https://github.com/nose-devs/nose/pull/1087/files. After submitting the pr I discovered a new version of the project (https://github.com/nose-devs/nose2/tree/master/nose2), and so I'll submit a similar pr to the other project as well.

### Week 6

**Current Stage: Bug Fix Submitted to Project**

I made a new fix for the nose2 version of the project, and submitted it here: https://github.com/nose-devs/nose2/pull/425. I had some trouble adding test files to the repository, so I posted a note in the pull request.
