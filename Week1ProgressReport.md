I spent a lot of time getting set up this week. Here is are the main pieces I spent my time on:

* Setting up a testing environment: I installed VMWare and set up an 32-bit Ubuntu image. The main challenge here was finding a supported 32-bit version.
* Setting up Crash Simulator: I installed rreplay and all dependancies. There were a couple of additional system configurations that I had to do to get everything working, then I encountered a bug (see below) and has to switch to the provided VMWare image.
* Submitting issues to rreplay: I submitted 2 issues [Pickle Regeneration fails in rrinit](https://github.com/pkmoore/rrapper/issues/32) and [Add support for openat](https://github.com/pkmoore/rrapper/issues/33)
* Additionally, I tested awk, ls, passwd, and tar but was not able to find a file type bug.
