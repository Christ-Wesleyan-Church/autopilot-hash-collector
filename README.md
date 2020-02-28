# AutoPilot Hash Collector
This is a simple wrapper script around Michael Niehaus's  [Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) PowerShell script for quickly collecting Windows AutoPilot device hashes from PCs with a flash drive.

The general idea is that you download this repo to a flash drive and then run `run.cmd` as admin. This will automatically download the latest version of Michael's script the first time it is run, and then create a `csv` file to which all of your hashes will be appended. This way, no permanent changes are made to the machine, there's no need to mess with changing the PowerShell execution policy, and no scripts are installed system-wide. Using this method, you can quickly collect hashes from large numbers of machines by pressing SHIFT+F10 to get a shell in OOBE.

Here's what this looks like:
![Image Demo](capture.gif)