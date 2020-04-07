# How to build:

Make sure that you have the required dependencies:

Mac:
- https://developer.mozilla.org/en-US/docs/Mozilla/Developer_guide/Build_Instructions/Mac_OS_X_Prerequisites

Windows:
- https://developer.mozilla.org/en-US/docs/Mozilla/Developer_guide/Build_Instructions/Windows_Prerequisites

Linux:
- https://developer.mozilla.org/en-US/docs/Mozilla/Developer_guide/Build_Instructions/Linux_Prerequisites

After cloning this repo:
- cd into the root folder of this repo
- run ./mach bootstrap
  - follow on screen instructions and select build for Firefox desktop (option 2)
- run ./mach configure
- run ./mach build
- run ./mach run
        
*Note if the bootstrap command fails on Mac try the following command instead:
- curl https://hg.mozilla.org/mozilla-central/raw-file/default/python/mozboot/bin/bootstrap.py > bootstrap.py && python bootstrap.py

This repo has the 3 out of the 5 issues implemented as outlined in our deliverable 2.
- Issue 1
  - https://github.com/mozilla/gecko-dev/commit/f11a8669892d8301b7ee4728f044ec161aa100cb
- Issue 2
  - https://github.com/CSCD01/gecko-dev-team09/commit/ebea7ea2abb4e75d730cf797ea061c140333056d
- Issue 3
  - https://github.com/CSCD01/gecko-dev-team09/commit/45693634c36d3f73fddd0ba9b5e147dfaf4b5fa2



If you have issues getting this repo to build for some reason you can also see our work by checking out the original mercurial repository and checking out the appropriate changesets:

# Checking out on Mercurial
To install mercurial:
On Mac: 
- brew install mercurial
On Unix/Linux:
- apt-get install mercurial

Cloning the mercurial repo:
- hg clone https://hg.mozilla.org/mozilla-central

Building:
- run ./mach configure
- run ./mach build
- run ./mach run
    
These are our issues with the corresponding revisions on mercurial:
- Issue 1: 516614:ad041092e560 
  - https://hg.mozilla.org/integration/autoland/rev/e01d0f2150c9
  - (Patch has already been accepted and is on the live version, so checking this would be unnecessary)
- Issue 2: 517069:f38f17bbbabe
  - https://phabricator.services.mozilla.com/differential/diff/242741/changesets/
- Issue 3: 518129:590212a8f409
  - (Another user's patch was accepted for this issue. You can see our implementation of this one in the github link above.)
  
  
  
# Project Feature
To check out our implemented project feature please check out the mozilla central project using mercurial using the steps above and checkout our revisions using the following command:
- hg update -r 520905

Official threads pertaining to our feature are found here:
- https://bugzilla.mozilla.org/show_bug.cgi?id=1528288
- https://phabricator.services.mozilla.com/D68708#change-yXY2hZewHp0D
