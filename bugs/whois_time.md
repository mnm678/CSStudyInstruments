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

### Week 3

The bug seems to be occurring during a socket call in whois that includes a timeout.

### Week 4

I don't think there's a way to address this issue without breaking the timeout.
