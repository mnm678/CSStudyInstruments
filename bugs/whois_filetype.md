## Meta
* Project: whois
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: Bug Identified
* Brief description (This can change as you progress) :

The whois command does not error when the filetype is changed to a IFDIR in crash simulator.


## Updates


### Week 2

**Current Stage: Bug Identified**

Bug discovered when changing file types in an fstat call with rreplay. I found the bug in the fstat call for `/etc/hosts`. The program seems to check for character devices and behave differently, but it does not check for a DIR.
