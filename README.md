## Security Risks
1. Administrator privileges  
OBS only recognizes plugins inside Program Files/Vstplugins. Moving files to programfiles requires administrator privileges.

2. Base64  
I inserted the zip file as Base64 into the code for offline installation without an internet connection. The internal files are:  
shell2vst64.exe, vst3shell.x64.core, vst3shell.x64.dll
