# Network Slice Selection Function XOS Service

It follows the standard XOS service implementation for CORD 4.0.

**Xproto models, Policies and Synchonizer code** are based in the default example service XOS model.

**Steps and Roles** for deploying the VNF are specific to the NSSF and include
- Database creation based on a MySQL Script
- IP configuration for NSSF VNF communication with vMME
- Definition of synchronizer functions for getting the IPs of Instantiated SPGW-C and SPGW-U (status of the network)  

Description of this section can be found [here](xos/synchronizer/steps)

This repo is part of a *CORD 4.0* deployment, the service needs to be cloned into the `cord/orchestration/xos-services/` directory before starting XOS.
After cloning, rename the folder to **nssf**

We plan to include a script to facilitate integration of this service with a CORD deployment.

## Acknowledgment
This research was supported by the MSIP (Ministry of Science, ICT and Future Planning), Korea, under the ITRC (Information Technology Research Center) support program (IITP-2017 2017-0-01633) supervised by the IITP (Institute for Information & communications Technology Promotion.
