# SEAPATH -  TSC Meeting

Thursday, Jan 2020, 2020 [60 minutes]  
Attendees(expected):  Aurelien Watare,Eloi Bail, Sander Jansen


## Organization

Note-taker - Rotate responsibility by meeting  Aurélien WATARE


### State of the project 

Reminder : 

* project Kanban is available [here](https://github.com/orgs/seapath/projects/1)

### Last time action

* Realeases ? What is the good policy ? 
* LTS / Real patches ?  A proposition will be made at the next TSC
* IEC61850 Tools:
  * License issue ?
    * .so ? 
* where to put the IEC61850 tools ?
  * Repository => sub-directory
* Secure boot : is it something that will be mainline ? YES

### Development:

New  features:

* configuration file
* extension of the no security distro to debug image
* possibility to disable IPV6

Working on :

ability to host a common CI for the project in RTE's lab
* hardware is in place 
* working on internet inbond access and security


### Discussion

* Long term test for the CI:
  * Linux tests
  * IEC61850 tests (business tests)

* real time issue with kernel 5.x

* IEC61850 tools : 
  * working on ELK dashboard and best way to collect the log without any impact on the experimentation

**release**

follow yocto rules => kingstone branch might be the base (April 2022)
minimum cores => minimum effort so all the features that are not identified as the core of the project should be maintain on a best effort basis
kernel =>  use only one version per release branch and follow the kernel lts evolution

Use the github tools to release the different version 



