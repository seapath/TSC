# SEAPATH -  TSC Meeting

Thursday, Jan 2020, 2020 [60 minutes]  
Attendees(expected):  Aurelien Watare,Eloi Bail, Tony Milne, Sander Jansen


## Agenda (proposal)

Note-taker - Rotate responsibility by meeting  Aurélien WATARE


### State of the project 

Reminder : 

* project Kanban is available [here](https://github.com/orgs/seapath/projects/1)

**Development**:

Done:

main :

* Realeases ? What is the good policy ? 
  *  LTS / Real patches ?  A proposition will be made at the next TSC
* IEC61850 Tools:
  * License issue ?
    * .so ? 
  * Organisation
    * Repository => sub-directory
* Secure boot : is it something that will be mainline ?
 

Doing:

rte-dev branch :

* VM backup
* monitoring tools to analyse Realtime performance : lttng + tracecompass ?
* integration of IEC61850 test tools (sample value stream generation to measure latency)

main :

* Check if no IOMMU image is still needed
* Kernel investigation regarding the RT bug (see below)

Bug :

* network not working for guest after some time (tap issue in kernel RT 4.19)
* Decide to merge to 5.15  on the main branch to solve the issue

**CI**

see mindmap
