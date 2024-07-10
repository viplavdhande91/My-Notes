## Azure Virtual Machines

### Scaling VMs
- **Single VMs**: For testing, development, or minor tasks.
- **Grouped VMs**: For high availability, scalability, and redundancy using scale sets and availability sets.

### Virtual Machine Scale Sets
- Create and manage identical, load-balanced VMs.
- Automated scaling based on demand or schedules.
- Centralized management, configuration, and updates.
- Automatic deployment of load balancers for efficient resource usage.
- Suitable for large-scale services (compute, big data, container workloads).

### Virtual Machine Availability Sets
- Ensure resilient, highly available environments.
- Group VMs by update domain and fault domain:
  - **Update Domain**: Groups VMs that can be rebooted simultaneously, ensuring only one group is offline during updates.
  - **Fault Domain**: Groups VMs by common power source and network switch, protecting against physical failures.
- No additional cost for configuring availability sets.

### Use Cases
- **Testing and Development**: Quick creation and deletion of different OS and application configurations.
- **Running Applications in the Cloud**: Economical benefits by handling demand fluctuations and paying only for used resources.
- **Extending Datacenter to the Cloud**: Virtual networks in Azure for applications like SharePoint.
- **Disaster Recovery**: Cost-effective IaaS-based approach for running critical applications during primary datacenter failures.

### Moving to the Cloud with VMs
- Lift and shift: Move from physical servers to the cloud with minimal changes.
- Maintain VM as with physical servers: Responsible for OS and software maintenance.