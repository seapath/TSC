# Roadmap SEAPATH

## Continous integration for Debian

### Write basic specifications

### V0.1 Structure of the CI is operationnal

- Orchestrator is operationnal (example GithubAction or Jenkin)
- Tests à the Host level
- The infrastructure is set up (real machines ready to be tested)
- The reference architecture is implemented (basically the reference network configuration)
- first tests are written in ansible playbook ( one scenario = one playbook) 

	- Realtime
	- Cybersecurity
	- Cluster

### V0.2 Integration of the Test VM

- A test VM that include tools to do IEC61850 tests

	- Sample Values 

		- Latency
		- number of streams that can be handled

### V0.3 -> V1

- enhanced tests for the Host
- enhanced test for  the VM tests

## Configuration and deployment

### Current state review

- First installation with Debian FAI
- Configuration of the cluster with Ansible
- deployment of the vm with vm-mgr
- WhitePaper about the philosophy

### Next (possible) step

- create a graphic tools that can manage the lifecycle of the configuration and deployment
- add a single node version
- improve documentation

## Cybersecurity

### Current state review

- WhitePaper about the philosophy

### V1 : reference for the debian version

- Based on ANSII NT-28 (french standard)
- test reports with the CI and cukinia (open source testing tool)

### Continuous improvement based on user needs 

- different flavors need to be tunable
- follow the standard policies

## Network

### Current state review 

- White paper about the strategy based on the needs (Linux Bridge / XDB, SR-IOV/ DPDK)

	- needs =

		- low consumption
		- performance 

			- no IEC61850 paquet loss inside the VM
			- latency < 500µs for xSV n Sv streams inside the TestVM

- description of the reference implementation

### implement reference implementation based on the white paper

## VM / RealTime

### Current state review

- White paper about the optimum configuration for IEC61850 based applications 

	- The cycle of the applications inside the VM is guaranteed while sharing a maximum of ressources with other 
	- The adherence with the host is miminimal

### VMtest architecture V0

- Simple application inside a VM to handle SV streams

### VMtests V1

- reference VM that include a reference architecture for a IEC61850 based application
- Guidelines to build  RT VM on SEAPATH

## supervision /monitoring

### Current state review

- White paper about the philosophy 

## External

### improve collaboration with the other project of the LF_ENERGy Foundation

### Define a communication strategy

