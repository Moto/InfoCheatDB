# Windows DISK


## Remove Write Protection
Use the Windows diskpart utility to remove write protection from the drive.
From the Command Prompt, type "diskpart", Enter, "list disk" and then Enter again. You'll see a numbered list of all disk volumes.

Find your USB drive by looking at the size of each volume and comparing it with your flash drive size. Type "select disk 1" or "select disk 2", etc. depending on the number Windows assigned to your USB drive. Press Enter.

Next, type this exact phrase, minus quotes: "Attributes disk clear readonly". Press Enter, wait for diskpart to do its work and then type "Exit" and Enter again.
