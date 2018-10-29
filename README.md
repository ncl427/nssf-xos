# Network Slice Selection Function XOS Service

It follows the standard XOS service implementation for CORD 4.0.

**Xproto models, Policies and Synchonizer code** are based in the default example service XOS model.

**Steps and Roles** for deploying the VNF are specific to the NSSF and include
- Database creation based on a MySQL Script
- IP configuration for NSSF VNF communication with vMME
- Definition of synchronizer functions for getting the IPs of Instantiated SPGW-C and SPGW-U (status of the network)  

This repo is part of a *CORD 4.0* deployment, the service needs to be cloned into the `cord/orchestration/xos-services/` directory before starting XOS.
After cloning, rename the folder to **nssf**

I plan to include a script to facilitate integration of this service with a CORD deployment.
