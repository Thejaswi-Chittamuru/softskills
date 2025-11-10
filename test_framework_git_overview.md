### Test Framework design

#### Libraries 

- Configs - libraries to apply configurations to DUTs or devices used
- Ops - to run show commands / fetch results from Devices
- parsers - to parse the formats from outputs returned by "show commands" ops.
- Utils - other utils

#### Test Scripts 

Entire script can be written in single class ( if all TCs are similar ) or Testcases can be grouped together based on tests / configs / etc into multiple classes in a single script file.

- setup class  - runs at beginning of class - used to initiate objects / basic configurations / basic checks ( device reachable / link checks / etc )
- teardown class - runs at end of class - cleanup of objects / base configurations
- setup method - runs before every TCs - any pre testcase initialization or verification - like protocols up , etc.
- teardown method - cleanup after every TCs
- Testcase - actual test - we create object for every library needed and call methods in library to write the testcase - object.method()

###########################################################################

### GIT

- git checkout - switch between branches
- git pull - pull from repo to laptop / local
- git push - push from laptop / local to repo
- git commit - commit to brach in laptop / local - by doing commit it will not reflect in repo - commit + push -> will reflect in repo
