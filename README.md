# Quick Recon PowerShell Script

## Description

The `quick-recon.psm1` PowerShell script is designed to perform quick network reconnaissance on a host. It provides a simple and informative overview of the host's configuration, domain information, IP details, and user accounts.

## Usage

1. **Import the Module:**
   - Run the following command to import the module:
     ```powershell
     Import-Module .\quick-recon.psm1
     ```

2. **Run Recon:**
   - After importing the module, execute the `Get-Recon` function to initiate the reconnaissance.
     ```powershell
     Get-Recon
     ```

3. **Output:**
   - The script will generate a file named `recon.txt` on the Desktop of the user who opened the PowerShell shell. This file contains relevant information about the host.

## Example

```powershell
PS C:\Users\MTanaka> Get-Recon

Directory: C:\Users\MTanaka\Desktop

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         11/3/2022  12:46 PM              0 recon.txt
```

## Notes

- This script utilizes the `ActiveDirectory` module for collecting domain information.
- The reconnaissance currently works only on the local host from which it is run.
- The output is saved to a file named `recon.txt` on the Desktop.

Feel free to explore and modify the script for your specific needs. Contributions and feedback are welcome!
