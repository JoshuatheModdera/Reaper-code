# Reaper-code
@echo off
color 6


title Joshua moding



:greeting
cls



ECHO    ########  ########    ###    ########  ######## ########  
ECHO    ##     ## ##         ## ##   ##     ## ##       ##     ## 
ECHO    ##     ## ##        ##   ##  ##     ## ##       ##     ## 
ECHO    ########  ######   ##     ## ########  ######   ########  
ECHO    ##   ##   ##       ######### ##        ##       ##   ##   
ECHO    ##    ##  ##       ##     ## ##        ##       ##    ##  
ECHO    ##     ## ######## ##     ## ##        ######## ##     ## 



set /p IP=Enter IP: :
:top
PING -n 1 %IP% | FIND "TTL="
IF ERRORLEVEL 1 (SET IN=0b & echo Downed.)
color %in%
ping -t 2 0 10 127.0.0.1 >nul
Goto top