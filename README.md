## Manual processing requirements
In order for OBS to automatically recognize VST3 using vst3shell and shell2vst, the following conditions should fulfilled.
- VST3 should installed via installer.
- vst3shell.x64.core and vst3shell.x64.dll should NOT be deleted or moved from initial location once shell2vst.exe executed.
- DLL file generated through shell2vst must be located inside Program Files/Vstplugins.
###
Executable Powershell script **automate** cumbersome processes.  
https://github.com/yln2/obsvst3/raw/main/vst3wrapper4obs.exe
###
## Security Risks
1. Administrator privileges
 OBS only recognizes plugins inside Program Files/Vstplugins. Moving files to programfiles requires administrator privileges.
2. Base64
 I inserted the zip file as Base64 into the code to install without an internet. The internal files are:
shell2vst64.exe, vst3shell.x64.core, vst3shell.x64.dll
