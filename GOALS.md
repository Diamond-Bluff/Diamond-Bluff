# **Detail Goals for Diamond Bluff**

* Create community-driven standards-based open ecosystem for DPU/IPU-like
  technologies
  * Establish an open community to support vendor-independent and jointly
    co-developed ecosystem
  * Build a truly open ecosystem that practices open source development
    principles and is always open to new members and contributors
  * Adhere to existing and commonly accepted open standards or help foster best
    practices in lieu of standards, as required
* Create vendor agnostic framework and architecture for DPU/IPU-based software
  stacks
  * Lifecycle management
    * BMC, secure boot, root of trust, loading, etc
    * Software installation, related security
  * System Integration Framework
    * Define operating environment
    * Software abstraction layer/framework
    * Support direct host access to DPU/IPU HW offloads
    * Support services distributed across host(s) and DPU/IPU(s)
  * Vendor-agnostic services
  * Telemetry → observability
* Reuse existing or define a set of new common APIs, when required, for
  * DPU/IPU hardware
  * DPU/IPU-hosted applications
  * Host Node
  * (Remote) provisioning software
  * (Remote) orchestration software
  * Configuration API per service
  * Consumption API per service
* Provide implementation examples to validate the architectures/APIs
  * Create technical papers and functional diagrams to help better understand
    the overall architecture(s)
  * Provide sample service implementations for validating frameworks
  * Develop reference proof of concept (POC) as well as simulation and test
    environments for testing APIs


# **Company-specific Goals**

### **Dell**
* Execution environment that supports DPU resident services
  * SONiC Network Services
  * Storage Services
    * Multi-path
    * File System
    * Data protection
    * NMVe-oF
  * a standard mechanism for integrating xPUs into server hardware management
    (e.g. iDRAC, HPE iLO, etc…) so customers aren’t buying Dell SKUs, HPE SKUs,
    etc…
  * Standard mechanisms for things like boot coordination and so on
  * Standards for Application deployment metadata where the app can describe
    what resources it needs from the xPU to ensure both compatibility as well as
    resource availability
  * Control Plane Offload
  * Security Services
    * DPI
    * Intrusion Detection
    * Firewall
* Multi-Vendor Open DPU Infrastructure API defined and adopted
  * system management
  * Telemetry configuration and delivery
  * Lifecycle
  * App and service deploy to the DPU
  * Hardware acceleration configuration & software developer kit access
    * i.e. a set of common Hardware Abstraction layers similar to SAI for SONiC
  * Storage
    * Networked Storage
      * NVMe/TCP
      * NMVe/RoCE(RDMA)
    * Storage Services
      * RAID/Erasure Coding/etc
    * Compression
    * SDXI Offload
  * Gateway
    * Connection Tracking
    * Load Balancing
    * NAT
    * Tunnels
  * Networking
    * SONiC
      * OpenConfig (includes BGP, etc)
      * SAI implementation by the DPU
    * Policing and QoS and SLA
    * Multi-tenant Overlay
    * Host facing NIC Configurations
    * OVS
  * Security
    * Policy & Filters
    * Crypto Offloads
    * Secure Storage
      * keys, secrets, attestation, …
    * Key Management
    * Network security offload
      * (TLS, IPSec)
    * RegEx matching


### **F5**
* F5 wants to see the creation of a multi-vendor, ISV friendly, DPU hosted
  software stack
  * Allows for ISV application portability across multiple DPU types
  * Allows an ISV application to access similar HW accelerations on different
    DPU’s using a set of common APIs
  * Provide a PaaS layer that is deployable across multiple DPUs to enable
    automated ISV application deployments, scaling, and manageability
* F5 wants to see the creation of an ISV friendly DPU ecosystem spanning the DPU
  enabled datacenter
  * Common provisioning APIs allowing for large scale, heterogenous, DPU
    deployments
  * Common management and telemetry APIs allowing for control, monitoring, and
    debug, of DPU’s instances at scale
* F5 wants to have an open, collaborative, and easy to consume DPU marketplace
  * Open Ecosystem – not a Walled Garden controlled by the largest vendors
  * Diamond Bluff frameworks and images that can be used without license or
    royalty burdens
  * Would like Diamond Bluff images – downloaded from Github – to work
    immediately without additional licensing steps required by one or more
    vendors


### **IBM**
* IBM wants to see the creation of a multi-vendor, ISV-friendly, DPU/IPU hosted
  software stack that
  * Allows for ISV application portability across multiple DPU/IPU types
  * Allows an ISV application to access similar HW accelerations on different
    DPU’s using a set of common APIs
  * Provides a PaaS layer that is deployable across multiple DPUs/IPUs to enable
    automated ISV application deployments, scaling, and manageability


* Create an ISV-friendly common set of management and control APIs for DPUs/IPUs
  * In the Diamond Bluff community, work towards consistent APIs for management
    and control of DPU/IPU cards, achieving consistency across a broad range of
    DPUs/IPUs and enabling use of
    * Common provisioning APIs allowing for large scale, heterogenous, DPU
      deployments
    * Common management and telemetry APIs allowing for control, monitoring, and
      debug, of DPU’s instances at scale

  * Standardization of:
    * Discovery and management of DPU/IPU Offload capabilities
    * Standardize ways in which a DPU’s/IPU’s Security, Networking, and Storage
      offload capabilities can be discovered
    * Secure Encryption of Data in Flight Processing Offloads to DPUs/IPUs
      * Enable offload of TLS
      * Enable offload of IPSec
    * Key Management of DPUs/IPUs
    * Container Networking Offloads to DPUs /IPUs
    * Enable offload of Virtual Switching (OVS) Data & Control paths
    * DPU/IPU management
    * DPU/IPU secure boot
    * a forwarding plane abstraction:
      * Southbound APIs for DPUs/IPUs
      * Tabled drive interfaces for southbound abstractions

  * Achieve broad industry acceptance of Diamond Bluff as the Open Source
    community for DPU/IPU projects.  Work with existing, adjacent Open Source
    projects in collaboration where it makes sense, encouraging their
    integration of common management APIs


### **Intel**
* Engage and grow a broader community for Diamond Bluff
  * Ensure we can find a foundation and home for Diamond Bluff to grow and
    flourish.
  * Add community members who are interested in growing the broader IPU/DPU
    ecosystem.
  * Work towards a healthy community that is self-sustaining and able to add new
    members and help to make them productive.
  * Prevent the explosion and bifurcation of the Diamond Bluff community by
    working to ensure we control the number of sub-projects, their scope, and
    the ease at which new members can work with them.
* Work to achieve management and control APIs for IPUs/DPUs
  * In the Diamond Bluff community, work towards consistent APIs for management
    and control of IPU/DPU cards, achieving consistency across a broad range of
    IPUs/DPUs.
  * Foster the ability to integrate management APIs across adjacent Open Source
    projects.
* Forwarding plane abstraction
  * Southbound APIs for IPUs/DPUs
  * Table drive interfaces for southbound abstractions.
  * Work with existing Open Source projects in collaboration where it makes
    sense.
* Achieve broad industry acceptance of Diamond Bluff as the Open Source
  community for IPU/DPU projects
  * Start with a few projects which are being brought into the broader project.
  * Grow the projects as the community desires.
  * Ensure the projects do not overlap and achieve consistency.


### **Marvell**
* Standardization of Security Offloads to DPUs
  * TLS Processing
    * TLS Handshake Offload (Asymmetric Crypto)
    * TLS Record Processing Offload (Symmetric Crypto)
    * TLS Proxy Offloads
    * TLS Forward Proxy
    * TLS Reverse Proxy
  * IPSec Offload
    * IPSec Gateway
    *  IPSec Tunnel Termination

* Standardization of Container Networking Offloads to DPUs
  *  Offload Virtual Switching Data Path
    * E.g. OVS Datapath Offload
  * Offload Virtual Switching Control Path
    * E.g. OVS Control Path offload
  * P4 Defined Data and Control Plane
    * P4 Runtime based control of Virtual Switch datapath

* Standardization of Storage Offloads to DPUs
  * NVME over Fabric

* Standardization of discovery and management of DPU Offload capabilities
  * Standardize ways in which a DPU’s Security, Networking and Storage offload
    capabilities can be discovered
  * Standardize ways in which Hosting Systems can offload above workloads to the
    DPU

* Standardization of DPU management
  * IPMI/redfish APIs etc.

* Standardization of DPU secure boot
  * Root of trust
  * Ehsm

“Standardization” = Vendor/Platform independent mechanisms for discovery,
configuration and offloading/scheduling of workloads to DPUs.


### **Red Hat**
* Define a set of hardware and software capabilities that shapes the future of a
  new class of cloud and datacenter infrastructure
* Develop a standard/common set of APIs that will spread across the variety of
  devices supported by the project
* Providing a consistent interface for users and applications to interact with
  DB-supported hardware
* Expand bare-metal and cloud-native platforms for deployments, management and
  orchestration of DB-accepted reference stacks (both HW and SW)
* Establish best practices for initialization of hardware, device enumeration
  and installation
* Architecting methods for accessing and utilizing features of DB-accepted
  hardware without crossing trust boundaries and maintaining security isolation


### **Individual Contributor**
TBD


# Other brainstorming materials and suggestions

* Create community-driven standards-based open ecosystem for DPU/IPU-like
  technologies
* Common APIs for offloading workloads[a]
  * Programmability (of services)
* Lifecycle management
* System Integration Framework
  * BMC, secure boot, root of trust, loading, etc
* Standard software abstraction layer for representation
* Software abstraction layer/framework
  * Define operating environment
  * Software installation, related security
  * Vendor agnostic services
* Telemetry → observability
