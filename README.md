@echo off
set d=C:\Windows\System32\getadministrator
goto AdminP
:AdminR
cls & echo You must have administrator rights to continue ...
pause >nul & exit
:AdminP
echo>%d%
if not exist %d% (goto AdminR) else del /f %d% >nul &cls
::your code here
