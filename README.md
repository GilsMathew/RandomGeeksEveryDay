# RandomGeeksEveryDay
A culmination of Learnings
------
- Date : 27 Sep 2021
- - - -
### Permissions on Registry Keys Using REGINI Command Windows
*REGINI command is present by default in windows OS. It can be used to set permissions on Registry keys.*

```bash
Command : REGINI <full path of script file>
```
##### **Steps**
**1.** Write script file where we add the registry key and the Permissions and save it with .txt extension.
  <br> The content of the script : RegistryKey [i] , where i is the security suffix. we can add multiple suffix in [] of the script.
  RegistryKey [i j k]
  ![setpermission](https://user-images.githubusercontent.com/46650581/134902318-0cd4c6f3-b035-42fa-b98c-7a811bb70307.JPG)
 
  The security suffix numbers is
  ```
  1  - Administrators Full Access
  2  - Administrators Read Access
  3  - Administrators Read and Write Access
  4  - Administrators Read, Write and Delete Access
  5  - Creator Full Access
  6  - Creator Read and Write Access
  7  - World Full Access
  8  - World Read Access
  9  - World Read and Write Access
  10 - World Read, Write and Delete Access
  11 - Power Users Full Access
  12 - Power Users Read and Write Access
  13 - Power Users Read, Write and Delete Access
  14 - System Operators Full Access
  15 - System Operators Read and Write Access
  16 - System Operators Read, Write and Delete Access
  17 - System Full Access
  18 - System Read and Write Access
  19 - System Read Access
  20 - Administrators Read, Write and Execute Access
  21 - Interactive User Full Access
  22 - Interactive User Read and Write Access
  23 - Interactive User Read, Write and Delete Access
  ```
**2.** Open Command Prompt in administrator privilege and run the command
  ```
  REGINI setpermission.txt
  ```
 - - - -
