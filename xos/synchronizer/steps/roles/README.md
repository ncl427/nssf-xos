## Roles description

This section contains the Ansible playbook instructions that are going to be applied when deploying the **NSSF Virtual Machine (VNF)**

The **pre-requirement** section sets the Linux Host name of the machine to *nssf* in order to easily identified in console.

The **nssf-configure** section has the actual playbook instructions for *VM deployment* and is organized as follows:
- defaults
- tasks
- templates

**Defaults** sets up some variables with pre-determined values that may be used during the VM deployment.
**Tasks** has the instructions that are going to be run as *console commands* (Like a Script) and will setup the VM with the right IPs and also create the **Slice Data Base** using *mysql*.
**Templates** Has the DB script that fills the Slice DB with actual values, using variables defined in the **Defaults** section and also the variables defined in the **Steps** Playbook File.

With this instructions the NSSF VNF can have the correct configuration before operation.
