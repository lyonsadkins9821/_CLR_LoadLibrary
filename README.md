# _CLR_LoadLibrary
cal $sXPTable_file = "c:\1\XPTable.dll" ;~  Local $sXPTable_file = "L:\CLRv1\XPTable.dll"     FileCopy($sXPTable_file, 'C:\Program Files (x86)\AutoIt3\', $FC_OVERWRITE)     ConsoleWrite("! " &amp; FileExists($sXPTable_file) &amp; @CRLF)     Local $oXPTable = _CLR_LoadLibrary($sXPTable_file) ;~  Local $oXPTable = _CLR_LoadLibrary("XPTable")     ConsoleWrite("+Object: " &amp; IsObj($oXPTable) &amp; @CRLF)      Exit
