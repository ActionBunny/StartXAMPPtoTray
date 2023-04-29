# StartXAMPPtoTray

.bat file in XAMPP dir with:

@ECHO OFF
ECHO start XAMPP and minimize to tray
start %~dp0xampp-control.exe
timeout 3 > NUL
powershell (ps xampp-control).CloseMainWindow()

and link that file to shell:startup
