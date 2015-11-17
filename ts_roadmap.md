In order to provide better experience to Galaxy users we plan to work on the following improvements.


Tool Shed side
---------

* refactor out dependency resolution to dedicated library
  * takes tool_dependencies.xml and generates a bash file
  * will also be used in Galaxy
* implement 'pull from github' functionality on TS repositories

Galaxy side
----------
* new UI for tool installation on the Galaxy side
  * using TS API
  * installed tool management UI
  * recognize suites
  * hide packages (tabs)
  * providing admin with a choice of dependency resolution plugin
* allow multiple ways of resolving dependencies on the Galaxy side
  * Tool Shed
  * easy_build
  * docker
  * guix
  * brew
  * conda


homebrew
------------
- prepare versioned homebrew-science tap (using the hackathon formula), possibly automated
- match all dependencies maintained by the MTS (~400 package* repos) to their counterparts in brew
- implement proof-of-concept galaxyside brew dependency resolution for one complex-enough tool (cufflinks?)



TS 2.0
-------
For new Tool Shed we would probably need to come up with 'good enough' (TM) conversion of tools from TS 1.0 to TS 2.0 that will improve the probabilty of being able to get rid of the TS 1.0 in the future
