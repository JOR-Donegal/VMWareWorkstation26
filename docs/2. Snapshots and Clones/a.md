# Snapshots
A snapshot (the term is taken from photography) is the ability to take a copy of the state of a system at a definite point in time. In most cases an actual copy is not taken, the management system uses clever mechanisms to track changes which expose the snapshot functionality; it looks like there is a copy, there isn’t!

When you take a snapshot, the original virtual disk (.vmdk) becomes read-only. All new changes go into a delta file (also called a redo log). These contain any blocks modified since the snapshot.

Taking a snapshot of a virtual machine saves its current state and enables you to return to the same state repeatedly. When you take a snapshot, Workstation captures the entire state of the virtual machine. You can use the snapshot manager to review and act on the snapshots for an active virtual machine.

Note that this process is not fool proof. Suppose you snapshot a VM when it is in the middle of a transaction. If you then revert to that snapshot at a later time, the VM may not be consistent with whatever happened during the transaction. It is best to take snapshots of a VM which is shut down and also it is best to use snapshots with VMs that do not keep state. Taking snapshots of a live database server could cause issues!

We will commonly use this functionality before doing updates, or installing software, or when any event is imminent which might threaten the integrity of the VM. Although we can make multiple levels of snapshot, we rarely do. We also keep our snapshots short-lived. This is because of performance implications. In this practical, you will take, revert and delete snapshots.

Databases and file systems may have the capability to support snapshots and most enterprise storage environments do.

## Exercise
1. Download “Using VMware Workstation for VMware Workstation X” from the VMWare site.
2. Review the section “Taking Snapshots of Virtual Machines”.
3. Clearly understand all the actions documented.
- Using Snapshots to preserve virtual machine states
- Using the Snapshot Manager
- Take a Snapshot of a Virtual Machine
- Revert to a Snapshot
- Deleting a Snapshot

List the files in the VM directory before taking a snapshot

Using your VM, exercise the above listed functions and test. During this process, check to see what file types are created, what size they are and whether they are deleted once you finish with the snapshots. Identify each file type and its extension.

## Testing
You should show that you have completed and tested the five specified topics. You should be able to draw some conclusions as to the application of this technique, where it might be used, duration, etc. Your records should demonstrate that you;
1. Use the methodology Research then Do, then Test and Document
2. Fully understand the implications of snapshots.
3. You understand their application, where and when to use them.
4. Know the file types to expect while you have live snapshots, before and after.