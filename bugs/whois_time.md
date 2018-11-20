## Meta
* Project: whois
* Project Bug Identifier:
* Link to Bug on Project Bug Tracker:
* Current Stage: Bug Identified
* Brief description (This can change as you progress) :

Whois fails if a gettimeofday call returns a different value.


## Updates


### Week 2

**Current Stage: Bug Identified**

Bug discovered when changing the result of time calls. The program appears to crash when gettimeofday returns certain changed values.
