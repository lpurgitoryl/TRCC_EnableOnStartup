# TRCC_EnableOnStartup
Enable Thermalright TRCC app on user login

- Go to Setings > Apps > Startup
  - Disable TRCC
- Start (Windows Key) > Command Prompt (Run as admin) > Then paste the command below (assumes default install location)
  - `schtasks /create ^
  /tn "\Thermalright\ThermalrightControl" ^
  /tr "\"C:\Program Files (x86)\TRCCCAPEN\TRCC.exe\"" ^
  /sc onlogon ^
  /rl highest ^
  /ru "INTERACTIVE" ^
  /f
`
## Credits
[Video Link](https://youtu.be/GMsUqOFeifs?si=tDKE1el_Sjaghc-r)
