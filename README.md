How to build:

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



  If you have issues getting this repo to build for some reason you can also see our work by checking out the original mercurial repository and checking out the appropriate changesets:
  
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
    
  If you wish to see our implemented issues please checkout the corresponding changesets on mercurial:
  - Issue 1: 516614:ad041092e560 (Patch has already been accepted and is on the live version, so checking this would be unnecessary)
  - Issue 2:
  - Issue 3: 517069:f38f17bbbabe
