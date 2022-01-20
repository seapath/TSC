# SEAPATH -  TSC Meeting

Thursday, Jan 2020, 2020 [60 minutes]  
Attendees(expected):  Aurelien Watare, Florent Carli, Eloi Bail, Mathieu Dupré, 


## Agenda (proposal)

Note-taker - Rotate responsibility by meeting  Aurélien WATARE


### State of the project 

Reminder : 

* project Kanban is available [here](https://github.com/orgs/seapath/projects/1)

**Development**:

Done:

main :

* Image/distribution refactoring
  * You can check the different flavors in the Readme
* Good practise:
  * to add a packet => image feature
  * to add a feature that is system wide => distro/machine feature

* example to build the  Sandbox distribution : `cqfd -b host-bios minimal` 

rte-dev branch:

* kernel 5.15 (network bug fix)
* ELK plugin
* net-snmp
* VM live migration
* Hawkbit patch
* ...

Good practise : 

* if a feature is mergeable => PR 
* if a feature is not in the core of the project (meta-seapath ) => create a different meta / add to another existing meta
* discussion needed about what should be in the meta-seapath core 

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
