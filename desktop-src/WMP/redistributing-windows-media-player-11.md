---
title: Redistributing Windows Media Player 11
description: Redistributing Windows Media Player 11
ms.assetid: 3348821f-6d72-40c2-954b-0046ce502401
ms.topic: article
ms.date: 4/26/2023
ms.custom: UpdateFrequency5
---

# Redistributing Windows Media Player 11

\[The feature associated with this page, [Windows Media Player SDK](/windows/win32/wmp/windows-media-player-sdk), is a legacy feature. It has been superseded by [MediaPlayer](/uwp/api/Windows.Media.Playback.MediaPlayer). **MediaPlayer** has been optimized for Windows 10 and Windows 11. Microsoft strongly recommends that new code use **MediaPlayer** instead of **Windows Media Player SDK**, when possible. Microsoft suggests that existing code that uses the legacy APIs be rewritten to use the new APIs if possible.\]

You can install Windows Media Player 11 on Windows XP by using one of the following setup programs, where *localeId* is a locale identifier.

-   wmp11-windowsxp-x86-*localeId*.exe
-   wmp11-windowsxp-x64-*localeId*.exe

Here is an example of a command line for installation with no UI and no restart or restart prompt.


```
wmp11-windowsxp-x86-enu.exe /q:A /c:"setup_wm.exe /Q /R:N"
```



The following table shows additional parameters that you can use with the Windows Media Player 11 setup program.



| Parameter              | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| /NoMigrate             | Prevent library migration.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| /NestedRestore         | Create a nested system restore point. Use this if your application creates a system restore point to nest the Windows Media Player restore point within your application restore point.                                                                                                                                                                                                                                                                                                                             |
| /DisallowSystemRestore | Disallow the creation of a system restore point. This flag will disable the creation of a system restore point. Under most circumstances this flag should not be used for general software redistribution. This should be used only when you can make an explicit choice on behalf of the end user not to support the rollback of the Windows Media Player files to an earlier version of the Player. This flag should be used only for corporate deployment or original equipment manufacturer (OEM) installation. |
| /DefaultService        | Set the initial online store.                                                                                                                                                                                     |



 

## Related topics

<dl> <dt>

[**Redistributing Windows Media Player Software**](redistributing-windows-media-player-software.md)
</dt> </dl>

 

 




