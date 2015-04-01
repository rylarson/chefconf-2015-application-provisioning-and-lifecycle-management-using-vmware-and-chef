# chefconf-2015-application-provisioning-and-lifecycle-management-using-vmware-and-chef

## Software Defined Datacenters
VMWare thinks everything in the datacenter should be modeled in software.

VMware & vCloud datacenter partners sits on top of a public and a private cloud. 

vRealize automation (we have this!)

"Model once, deploy anywhere"

Can deploy on vCenter, Azure, AWS. VMWare management solutions work with the public clouds, (hyperV, KVM, AWS, Azure, OpenStack)

You can model tiered application deployment with dependencies, etc. 

"Reservations" are an abstraction of resources. Set up AWS and Vcenter reservations.

Can grant permissions to Chef
Chef recipes can be included in the "Self service catalog"

vRealize Orchestrator plugin will be available soon. 

   Install Chef client and register nodes
   OS configurations
   Deploy and Configure Applications
   Deregister nodes and teardown

   Plugin features
       Support for Windows and Linux
       Support for multiple versions of cookbooks
       Applying a run list and setting attributes
       Integration with hosted and on-premise chef
       Edit data bags through VRO! Holy Fuck!

Active Network VRO Ruby Library

    Integrate Chef with the Application Blueprinting. I wonder if this is better than Terraform. I want to say no for our uses because VRO is all about "Managing the infrastructure" and we are not using VMWare to manage any long lived production infrastructure.


Define Chef org in a business group inside of vRA. 
Set properties on a clone operation inside of a BluePrint. (I will need admin access to vRO for shizzle.)

Then when requesting from that Blueprint, it prompts for properties we defined (e.g. environment, node name and RUN LIST!)

TODO Give a presentation on this with a POC and with a recording of this workshop.
TODO Send out the recording of this workshop.

vRA will add DNS records too. Sweet!

Tag a node in vRO and it gets tagged in Chef server

When you delete the VM it deletes the client and the node out of the Chef server

Worry: Can we do this with Chef solo?

This is supported by Chef and VMWare
