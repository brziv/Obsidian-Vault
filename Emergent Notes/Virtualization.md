#system 

Host machine --> Host OS -> Application <--- Physical machine
	|
	|---> Hypervisor -> Guest machine -> Guest OS -> Application <--- VM

Create isolated environments on one physical machine
	VM: software-defined computer
	Snapshot: state at a point
	Portability: move VM with config and OS
	Guest OS: run within a VM
	Hypervisor: manage VM-hardware interaction
	Server consolidation: multiple servers -> single, more powerful cluster