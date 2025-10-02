## Sorting data
Sort the flags in alphabetical order in /challenge/run , and you'll get the real flag in last. 

## My solve
**Flag:** `pwn.college{4cVkYCJMO1XQfScbb7LWkfceW36.0FM0MDOxwSOzgjNzEzW}`

Use sort to sort the flags in alphabetical order, you don't need to give any specific argument except the path of the file cuz by default
sort , sorts the data in alphabetical order. The flag for the challenge will be in the end of the sorted data.

```bash
hacker@data~sorting-data:~$ sort /challenge/flags.txt
ovm.collefe{4cVkYBJMO0XPfSbab7LWkfcdV25.0FM0LDOwvSOzgjNyEzW}
ovn.bollefe{4bVjYCIMO1XQfScbb7LWkfceW36.0FM0MDOxwSOzgjNzEzV}
ovn.bollegd{4cVjYCIMN1XQfScab7KWjeceV36.0FM0MCOwwSOzgiNyEzV}
ovn.cnkkefe{3bUkYCJMO1XQfScbb7LWjfbdW36.0FM0MCOwvSOygiMyEzW}
ovn.cnllege{4cVkYBILO1XPfRbab6LWjfcdW26.0EM0LDNxwSOzgiMzEzW}
ovn.colldfe{3bVkYBJMO1XPeScba7KWkfceW35.0EM0MDOwwSOzfjNyEyW}
owm.bollefe{4cUjYBJLO1XQeScab7LVjfceW35.0EM0MCOxvSNzgiMyEzW}
owm.cnkldge{4cUkXBIMN1XQfRcaa7KVkecdW25.0FM0MDOxwSNyfjNzEyW}
owm.colkegd{3cVjYCJLN1XQfScbb7LWjebeW25.0EM0LDOxwSOzfiMzEyW}
owm.colldfd{4cVjYBJMO1XQfScab6KVkeceW26.0FM0MCOwwSOzgjNyEyW}
own.bokkefd{4cVkYBJMO1XQeScbb7LWjfceW36.0FL0MCOxvSOyfjNzEyV}
own.boklefe{4cVkYBJLO0WPeScba7LWjebeW36.0EM0MDOxwROygjNyEyV}
own.boklege{3cVkYCILN0XPeRcab6LWkfceW26.0FM0MDOwwROzgjMzEzW}
own.bolldge{4cVkYCJMO1XQfSbbb7LWkfceW36.0FM0MDOxwSOzfjNzDzW}
own.cokldge{4cVkYBIMO1XQfScbb7LWkfceW36.0EM0LDOxwSOzgjNzEyV}
own.coklege{3bVkYCJMO1XQfScba6KWkfceW36.0EM0LDOxwSNzfjNzDzV}
own.colkefe{4cUkYBJLN1WQfSbbb7LWkfbeV26.0FL0LDOwwROygjNzDyW}
own.colkege{3cVkXCJMN1XPfRcbb7KVjfceW36.0FM0LDOwwSNygiMzEyW}
own.colldfd{3cVkXCJMO0WQfRbbb7LWjfceW26.0FL0LDOwvSOygjNzEzW}
own.collefe{4cUkYCILO0XQfScbb7LWjeceW36.0FM0LDOxvSOygiMzDzW}
own.collegd{4cVkYBJMO1XPfScbb7LWkfceW36.0EL0MCOxvSOygjNzEzW}
own.college{4cVkYCIMO0WQfScbb7LWkfcdW36.0FL0MDOxwSOzgjNzEzW}
own.college{4cVkYCJMO1XQfScbb7LWkfceW36.0FM0MDOxwSOzgjNzEzW}
pvm.bollefe{4cUkYCJMO1XPeSbbb7KWkfceW36.0EL0LCNxwSOzfiNzEzV}
pvn.bollefd{3cVkXBJLO1XQfScba7LWjebdW26.0FM0LDOxwSOzfjNzEzW}
pvn.cnkldfd{4cUkYCIMN1XPfScba7LWjfbeW36.0FM0MCOwwSOzgiNzEzW}
pvn.cnllefe{4cVkYCIMO1XPeScbb7LVjfceW36.0FM0LDNxwSNzgjNzDyV}
pvn.cokldge{4bUjXCJMN1XQeSbba6LVjfceW36.0FM0MCNxwSNzfjNyEyW}
pvn.coklefe{4bVkXCJLO1XPeScaa7LWjfcdW36.0FM0LCNwwSOygjNyDzW}
pvn.colkege{4cVkYBJMO0XQfScbb7LWkfcdW36.0FL0LDOxwSOzgiNzEzV}
pvn.collefe{4bVkYCIMO1XQfScbb7KWkeceW35.0EM0MCOxvROzfiNzDzW}
pvn.college{4bVkYCJLO1XQfScab7KWkfceW36.0FM0MCOxwROzfjNzEzW}
pwm.bolkdfe{4bVkYBIMO1WQfRcab6LWkfcdW36.0FL0LCNxvROzgjNyDzW}
pwm.cnkldge{4cVkYBJMO0XPfSbab7LWjfceV25.0FL0LDNxvROyfjNyDzV}
pwm.cnklegd{4cVkYBJMO1WPfScba7KWkfceW36.0FM0MDNxvSNygjNyEzV}
pwm.colkdge{4cUkYCJMO1XPfScbb6KVkecdV36.0FM0MCNwwSOzgjNzDzW}
pwm.college{4cVjXCJMN1XQfScab7LWkfceW36.0FL0MDOxwROygjMzEzW}
pwm.college{4cVkYCIMO1XQfScab6LVkfceW36.0FM0MDOxwSOzfjMyDzW}
pwm.college{4cVkYCJLO1XQfScbb7LWkfceW36.0FM0MDOxwSOzgjNzEzW}
pwm.college{4cVkYCJMO1XPeScbb7KWjfbeW36.0FL0LDOwwSOzfjMyEzW}
pwn.bnklege{4cVkYCJMN1XQeScbb7LVjfcdV36.0FM0MDNxvSOygjMzDyV}
pwn.bnlkdgd{3cVjYCIMO1XQfScba7LVjebeV26.0FM0LDOwvSOzfjNzDzW}
pwn.bnlkege{3cVkXCJMO1XPfScbb7KWkeceV36.0FM0MCOxwROzgjNzDzW}
pwn.bnllefd{4bUkYBJLN0XPfRcbb7LWjfceV36.0FM0LDNxvSNzfjMzEzW}
pwn.bnllege{4bVjXBIMO1XQfScbb6LVkfbeW26.0FM0LDOxwSNzgjNyEzW}
pwn.boklege{3bUkXCJMN0WPfRbab7LWjfceV36.0FM0MDNxvSOzfjNzEyV}
pwn.bolkefe{4bUkYCJMO1XPfRcbb7KWjfbeW35.0FL0MDOwwSOzgjNzEzV}
pwn.bolkege{4cVkYCJMO1XQfScbb7KWkfbeW36.0EL0MDOxwSOzgjNzEzW}
pwn.bolldgd{4cVkYCJMN1XPeScba7LVkfceW35.0FM0MDOwvSOyfjNyEyW}
pwn.bollege{4cVkYCJMO1XQfScbb7LWkfceW36.0FM0MDOxwSOzgjNzEzW}
pwn.bollege{4cVkYCJMO1XQfScbb7LWkfceW36.0FM0MDOxwSOzgjNzEzW}
pwn.cnkldge{4cVkYCJLN1WQfRbbb6LVkfceV35.0FM0LDNxwSOygjMzDzW}
pwn.cnklefd{4cVjYCJMN1WQeSbaa7LWkfceV36.0FM0MDOxwROyfjNyDyV}
pwn.cnklege{4cVkXCJMN1WQfScbb6LWjfceV36.0FM0MDNwwSOygiNyEyW}
pwn.cnlkdge{4cVkYCJMO0XQfRbbb7LVkecdV25.0FM0MDOxwSOzfjNzDzW}
pwn.cnlkefe{4cVkYCJMN1WQfScbb7LVkfceW35.0FL0MDOwwROygiMzEzV}
pwn.cnlldfe{4bVjYCJMN1XPfScbb7LWkfceW26.0FL0MDOxwSOzgiNzEzV}
pwn.cnllegd{4cUkXCJMO1XPfScaa7LWkfcdW36.0FM0MDOwwSOzgjNyDzW}
pwn.cnllegd{4cVjYCJLO1XPeScab7LWjebeW36.0FM0LDNxwSNzgjMzEyV}
pwn.cokkdge{4cUkXBIMO0WPeRcaa7LWkfcdW26.0FM0LDNxwROzgiNyDzV}
pwn.coklege{4cUkYCIMN1XQfRcbb7LVkfceW35.0FM0MDOxvSOzgjNzEzW}
pwn.coklege{4cVkXBJLO1WPeSbbb7LWkfbeW36.0FM0LDOxwSNygiNzEzV}
pwn.colkdgd{4cVkYCJMO1WQfScbb6KWkfceW26.0FM0LDOxwSOzfjMzEzW}
pwn.colkege{4bVkYCJMO1XQeScab6LWkfcdV26.0EM0MDNwwROygjNzEzV}
pwn.colkege{4cVkYCJMO1XQfScbb7KWkfceW36.0FM0MDOxwSOygjNzEzW}
pwn.colkege{4cVkYCJMO1XQfScbb7LWkfceW36.0FM0MDOxwSOzgjNzEzW}
pwn.colldge{3bVkYCJMO1XQfScbb7LWkfceW26.0FM0LCNwwROzfjNzEzW}
pwn.colldge{4cUjYBJLN0XPfRcbb6LWjeceV25.0FL0MDNxvSNzgjNzEyW}
pwn.colldge{4cVjYCJMO1XQfScbb7LVkecdW36.0FM0LDOxwSOzgjNzDzW}
pwn.collefe{3bVkYCJMO1XQfScbb7LWkeceV35.0FL0MCOxwSOzgjNzEyW}
pwn.collefe{4cUkYCJMO0XQfScbb7LWkeceW35.0FM0LDOxvSOzfjNyEzW}
pwn.collefe{4cVkXCJLO1XQfSbaa7LWkfceW36.0FM0MDOxwROzgiNzDyV}
pwn.collefe{4cVkYCJMO1XQfScbb7LWkfceW36.0FM0MDOxwSOzgjNzEzW}
pwn.collegd{3bUkXCJMN1XPfScba7LWkfceW36.0FM0LDOwwSOzfjNzEzW}
pwn.collegd{3cVkYCJLO1XQfScbb7LWkfceW35.0FM0MDOxwSOzgiNzEzW}
pwn.collegd{4cUkYCJLN1WQfScbb6KWkfcdW36.0EM0MDOwwROzgiNzEzW}
pwn.collegd{4cUkYCJLN1XPfScab7LWkeceW35.0FL0MDOxwSOzgjNzEzW}
pwn.collegd{4cVkXCJMN1XQfScbb7LWkfceW26.0EM0MDOxvROzgjMyEyW}
pwn.college{3bVkXCIMO1XQfScbb7KWkfceW26.0FL0MCOxwSNzgjNyEzW}
pwn.college{3cVkYCJMO1XQeSbbb7LWkfceW26.0FM0MDOxwSOzgjNzEzW}
pwn.college{4bVkYCJMO1XQfScbb7LWkfceW36.0FM0MDOxwSOzgjNzEzW}
pwn.college{4cUjYCJMO1XQfScbb7LVkfceW36.0FM0MDOxwSOzgjNzDzW}
pwn.college{4cUkYCJMO1XQfRcbb7LWkfceW36.0FM0MDOxwSOygjMzEzW}
pwn.college{4cVjYCJMO1XPfScbb7LWkfceV36.0FM0LDOxwSOzgiNzEzW}
pwn.college{4cVkXCJMO1WQfSbbb7LVkfbeW35.0EM0MDOxwSOygjNzDzW}
pwn.college{4cVkYCIMO1XQfScbb7LWkfceW36.0FM0MDOxwSOzgjNzEzW}
pwn.college{4cVkYCJLO0XPeSbbb7LVkeceW26.0FM0MDOwvSOzfjNzDyW}
pwn.college{4cVkYCJLO1XQfScbb7LWkfceW36.0FM0MCOxwSOzgjNzEzW}
pwn.college{4cVkYCJMO0XPfScbb7LWkfceW36.0FM0MDOxwSOzgjNzEyW}
pwn.college{4cVkYCJMO1XQfRcbb7LWkfceW36.0FM0MCOxwSOzgjNzEzW}
pwn.college{4cVkYCJMO1XQfRcbb7LWkfceW36.0FM0MDOxwSOzfjNzEzV}
pwn.college{4cVkYCJMO1XQfScba7LWkfceW36.0FM0MDOxwSOzgjNzEzW}
pwn.college{4cVkYCJMO1XQfScbb7KWkfceW36.0FM0MDOxwSOzgjNzEyW}
pwn.college{4cVkYCJMO1XQfScbb7LVkfceW26.0FM0MDOwwSNzgjNzEzW}
pwn.college{4cVkYCJMO1XQfScbb7LVkfceW36.0FM0MDOxwSOzgjNzEzW}
pwn.college{4cVkYCJMO1XQfScbb7LWkfceW35.0FM0MDOxwSOzgjNzEzW}
pwn.college{4cVkYCJMO1XQfScbb7LWkfceW36.0FM0MCOxwSOzgiNzEzW}
pwn.college{4cVkYCJMO1XQfScbb7LWkfceW36.0FM0MDOxvSOzgjNzEzW}
pwn.college{4cVkYCJMO1XQfScbb7LWkfceW36.0FM0MDOxwROzgjNzEzW}
pwn.college{4cVkYCJMO1XQfScbb7LWkfceW36.0FM0MDOxwSOzgjNzDzV}
pwn.college{4cVkYCJMO1XQfScbb7LWkfceW36.0FM0MDOxwSOzgjNzEzW}
hacker@data~sorting-data:~$
```

## What I learned
Learned about the sort command which is used to sort the files in order.<br>
There are specific arguments for specific orders : <br>
-r: reverse order (Z to A)<br>
-n: numeric sort (for numbers)<br>
-u: unique lines only (remove duplicates)<br>
-R: random order<br>

## References
None
