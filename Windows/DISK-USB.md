# Windows DISK & USB

## Check S.M.A.R.T. Status
In Windows, you can manually check the S.M.A.R.T. status of your drives from the Command Prompt. Just type "cmd" into the search bar on the taskbar and open the application. In the pop-up box, run the following:

```console
wmic diskdrive get model,status
```

It will return Pred Fail if your drive's death is imminent or OK if it thinks the drive is doing fine.

## Remove Write Protection
Use the Windows diskpart utility to remove write protection from the drive.
From the Command Prompt, type
```console
diskpart
```
Enter,
```console
list disk
```
and then Enter again. You'll see a numbered list of all disk volumes.

Find your USB drive by looking at the size of each volume and comparing it with your flash drive size. Type
```console
select disk #
``"select disk 1" or "select disk 2", etc. depending on the number Windows assigned to your USB drive.
Press Enter.

Next, type this exact phrase:
```console
Attributes disk clear readonly
```
Press Enter, wait for diskpart to do its work and then type
```console
Exit
```
 and push Enter again.
