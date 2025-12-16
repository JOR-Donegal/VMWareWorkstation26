# Clones

Installing a guest operating system and applications can be time consuming. On a recent install of Windows Server, the installation took several days (patching, reboot, more patching, corporate branding, hardening). With clones, you can make many copies of a virtual machine from a single installation and configuration process. Cloning a virtual machine is faster and easier than copying it. A clone is a full copy of a parent VM; an existing VM created previously. Crudely, we could just copy the entire folder of a VM, rename the folder and we have created a clone. There are cases where we do this. However, it can cause us problems, and these should be discussed with your lecturer. As a quick summary, many modern computers generate globally unique IDs (GUID) for resources and rely on them being unique. If we crudely copy a VM, these GUIDs are no longer unique. Another issue is network cards. Every Ethernet card in the world has a unique address. If you make a direct copy of a VM, both will have the same Ethernet address in their network cards.

A linked clone is harder to explain; it’s a combination of a snapshot and a clone. It is a unique virtual machine, but it shares virtual disks with a parent VM. Linked clones are really useful for doing lab exercises; we can create a linked clone in seconds and delete it when we are done. Clones are useful when you must deploy many identical virtual machines. Typically, when we build a virtual host, we will create gold images of each OS and clone from these images. If I need a new Windows Server file server, it will take hours or days to build from scratch. It will take a few minutes to clone form an existing VM.

## Research
Download “Using VMware Workstation X Pro” from the VMWare site. Review the section “Cloning Virtual Machines”.

Understand;
- Linked Clones
- Full Clones
- Template Mode

You should have an existing Linux client and server which are fully updated. Shut them down.

There is a description field for each VM, ensure you document the VMs before cloning.