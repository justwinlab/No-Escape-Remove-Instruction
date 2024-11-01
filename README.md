
# Instructions pour Modifications du Registre Windows

## Étape 1 : Importation des fichiers nécessaires
Importez les fichiers suivants :
- **SOFTWARE** : `C:\windows\system32\config\SOFTWARE`
- **SYSTEM** : `C:\windows\system32\config\SYSTEM`
- **USER** : `C:\users\Nom D'utilisateur\NTUSER.DAT`

## Étape 2 : Modifications du registre Windows

### Clé de registre : `Scancode Map`
- **Emplacement** : `HKLM\SYSTEM\CurrentControlSet\Control\Keyboard Layout\Scancode Map`
- **Action** : Supprimer la clé.

### Clés de registre pour les fichiers exécutables
- **Emplacement** : `HKLM\SOFTWARE\Classes\exefile\shell\open\command`
  - **Valeur** : Supprimer la valeur de "WINIT32".
- **Emplacement** : `HKLM\SOFTWARE\Classes\exefile\shell\runas\command`
  - **Valeur** : Supprimer la valeur de "WINIT32".

### Paramètres du système
- **Emplacement** : `HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System\EnableLUA`
  - **Action** : Mettre la valeur à **1** (pour activer l’UAC).
- **Emplacement** : `HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\Explorer\UseDefaultTile`
  - **Action** : Supprimer la clé.
- **Emplacement** : `HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System\shutdownwithoutlogon`
  - **Action** : Supprimer la clé.
- **Emplacement** : `HKLM\SOFTWARE\Policies\Microsoft\Windows\System\DisableLogonBackgroundImage`
  - **Action** : Supprimer la clé.

### Clés du registre utilisateur
- **Emplacement** : `HKCU\Software\Microsoft\Windows\CurrentVersion\Policies\System\DisableRegistryTools`
  - **Action** : Supprimer la clé.
- **Emplacement** : `HKCU\Software\Policies\Microsoft\Windows\System\DisableCMD`
  - **Action** : Supprimer la clé.

### Dernières modifications à la fin
- **Emplacement** : `HKEY_CURRENT_USER\Control Panel\Desktop\AutoColorization`
  - **Action** : Supprimer la clé.
- **Emplacement** : `HKEY_CURRENT_USER\Control Panel\Mouse\SwapMouseButtons`
  - **Action** : Supprimer la clé.
- **Emplacement** : `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon\AutoAdminLogon`
  - **Action** : Supprimer la clé.
- **Emplacement** : `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon\AutoRestartShell`
  - **Action** : Supprimer la clé.
- **Emplacement** : `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon\DisableCAD`
  - **Action** : Supprimer la clé.
- **Emplacement** : `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon\Userinit`
  - **Action** : Supprimer la clé.
