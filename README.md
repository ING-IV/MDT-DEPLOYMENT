Prueba de capture limpia Windows 11 24h2  crea un task.  Syspre and capture



Recuerda que la maquina que tenga  para capturar no debe estar en un-Domain 



 te comparto mi CustomSettings.ini

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


<img width="940" height="803" alt="Image" src="https://github.com/user-attachments/assets/087cdb26-97a6-4e60-b780-8895a4e19b02" />













Ver imagen agregar un Run Command Line  
Bajo el nombre   Reset Syspre state
Comand
cmd /c "echo. & echo Resetting Sysprep state... & reg add "HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Setup\State" /v ImageState /t REG_SZ /d "IMAGE_STATE_GENERALIZE_RESEAL_TO_OOBE" /f & C:\Windows\System32\Sysprep\sysprep.exe /generalize /oobe /shutdown /quiet"

 

<img width="940" height="733" alt="Image" src="https://github.com/user-attachments/assets/36d04286-982a-4e4a-af59-b661bc8b8880" />

ejecutar litetouch desde la maquina que queremos capturar  mapear la ruta  y correr la task 

<img width="994" height="780" alt="Image" src="https://github.com/user-attachments/assets/6a01a45a-a89c-4cd6-8778-17c2ed9faae5" />


<img width="940" height="659" alt="Image" src="https://github.com/user-attachments/assets/324cfb66-2bc5-4bf0-a78d-e8434d5c12a2" />

<img width="940" height="772" alt="Image" src="https://github.com/user-attachments/assets/bfca2d99-4c62-4b3d-a6ca-018b5a38ada0" />

 

 
