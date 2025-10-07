# MDT-DEPLOYMENT
Soluciones de Implementacion de windows  11
Prueba de capture limpia Windows 11  24h2  crea un task. 

Recuerda que la maquina que balla a capturar no debe estar en un Domain 
mi custum.ini

Custom [Settings]
Priority=Default
Properties=MyCustomProperty

[Default]
OSInstall=yes
oscapture=yes
SkipCapture=NO
SkipAdminPassword=YES
SkipProductKey=YES
SkipComputerBackup=NO
SkipBitLocker=YES


 <img width="940" height="733" alt="image" src="https://github.com/user-attachments/assets/53883dee-2a15-47d2-bcb1-4b1ebbf35f10" />














Ver imagen agregar un Run Command Line  
Bajo el nombre   Reset Syspre state
Comand
cmd /c "echo. & echo Resetting Sysprep state... & reg add "HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Setup\State" /v ImageState /t REG_SZ /d "IMAGE_STATE_GENERALIZE_RESEAL_TO_OOBE" /f & C:\Windows\System32\Sysprep\sysprep.exe /generalize /oobe /shutdown /quiet"

<img width="940" height="772" alt="image" src="https://github.com/user-attachments/assets/d1df8218-9fa3-44e1-af94-41fe4a1a2041" />
<img width="940" height="659" alt="image" src="https://github.com/user-attachments/assets/0cb90c10-c1e7-44e1-bb27-639a15a21f0e" />


 



 

