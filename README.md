# StringRepeat
 ConsoleWrite ("dictionnary = {" &amp; @CRLF) PrintDict($dict, 1)  Func PrintDict ($oDic, $lvl)   For $i = 0 to $oDic.count - 1     If IsObj($oDic.items[$i]) Then       ConsoleWrite (_StringRepeat(@TAB, $lvl) &amp; $oDic.keys[$i] &amp; ": {" &amp; @CRLF)       PrintDict($odic.items[$i], $lvl+1)     Else       ConsoleWrite (_StringRepeat(@TAB, $lvl) &amp; $oDic.keys[$i] &amp; ": " &amp; $oDic.items[$i] &amp; @CRLF)     EndIf   Next   ConsoleWrite (_StringRepeat(@TAB, $lvl-1) &amp; "}" &amp; @CRLF) EndFunc
