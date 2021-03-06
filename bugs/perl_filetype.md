## Meta
* Project: perl
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: Bug Fix Submitted to Project
* Brief description (This can change as you progress) :

The perl command does not error when the filetype is changed to a FCHR in crash simulator.


## Updates


### Week 2

**Current Stage: Bug Identified**

Bug discovered when changing file types in an fstat call with rreplay. When the input file is changed to a character device or directory the behavior does not change.

### Week 3

**Current Stage: Source of Bug Diagnosed**

perl does not appear to check the file type (or even extension) before trying to execute a script. In `pp_ctl.c` in the perl source, it appears to check for a directory or block device, but no other file types.

### Week 4

**Current Stage: Bug Fix Implemented**

After more investigation, it appears that the script is opened in `perl.c`. I changed the check to fail on any non-regular file. I started testing the fix, and it should be ready to submit soon.

### Week 5

**Current Stage: Bug Fix Implemented**

I wrote the fix and will submit the pr next week.

### Week 6

**Current Stage: Bug Fix Submitted to Project**

Perl takes patches through their email list, so I submitted the patch there.
