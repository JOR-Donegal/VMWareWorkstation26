# Full Clone
Create a full clone of the existing server VM

- Check how long it takes
- Examine the disk files afterwards, for both the parent and child VM.
- Call the new VM OS-L00xxxxxx where;
    - OS is the OS type, for example UB2404
    - L00xxxxxx is your L number

Restart and test the parent and child VMs.

- Can they all use the network?
- Check the MAC address of the network card on both.
- Are they the same?

Update the description in VMWare Workstation

# Linked clone
Make a linked clone of the existing client VM.

Check how long it takes.

Examine the disk files afterwards, for both the parent and child VM.

Call the new VM OS-L00xxxxxx-Date where;
- OS is the OS type, for example UB2404
- L00xxxxxx is your L number
- Date is todays date.

Linked clones are normally ephemeral, putting a date on is a useful note to yourself that this can be deleted once used.

Restart and test the parent and child VMs.
- Can they all use the network?
- Check the MAC address of the network card on both.
- Are they the same?

You should be able to draw some conclusions as to the comparative efficiency and application of full and linked clones.

Delete the linked clone and clean up as you are finished.