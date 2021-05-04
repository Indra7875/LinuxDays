### Day3
### Manual Structure

| Section 	|            Contains           	|                                                   Description                                                  	|
|:-------:	|:-----------------------------:	|:--------------------------------------------------------------------------------------------------------------:	|
|    1    	|         User Commands         	| Commands that can be run from the shell  by a normal user (Typically no administrative privileges are needed)  	|
|    2    	|          System Calls         	|                         Programming functions used to make calls to the  Linux Kernel.                         	|
|    3    	|      C Library Functions      	|               Programming functions that provides interfaces to  specific programming libraries.               	|
|    4    	|   Devices and Special Files   	|                     File system nodes that represent hardware devices  or software devices.                    	|
|    5    	| File Formates and Conventions 	|                    The structure and format of file types or  specific configuration files.                    	|
|    6    	|             Games             	|                                          Games available on the system                                         	|
|    7    	|         Miscellaneous         	|                   Overviews of miscellaneous topics such as protocols, filesystem and so on.                   	|
|    8    	|     System Administration     	|                     Commands that require root or other administrative  privileges to use.                     	|

* __Note :__ <br>
-- Sections 1,5 and 8 are what you likely use most often. <br>
-- In man page if something in '[ ]' then it is optional. <br>
-- In man page anything under '<>' is mandatory. <br>
-- In man page if '|' (pipe character) is there then it work as 'OR' operation. <br>
-- In man page if ... (ellipsis) is there then it will take more than one input. <br>
-- When you making long form option the words separated in below structure. <br> <br>
  ```
  $ ls -l --human-readable
  ```
---
```
$ man -k which
```
-- It will search the mannual page for 'which' input.
```
$ man 1 which
```
-- It will open mannual page for 'which' input in section 1.
```
$ man which
```
-- It will open mannual page for 'which' input.
```
$ which date cal
```
-- It will display the location of given input command.

#### Command Synopsis :

|      Section     	|                              Meaning                              	|
|:----------------:	|:-----------------------------------------------------------------:	|
|      [THING]     	|                         THING is optional.                        	|
|    < THING >     	|                   THING is mandatory (required)                   	|
|     THING ...    	|                THING can be repeated (limitlessly)                	|
| THING1 \| THING2 	|                  Use THING1 OR THING2. Not Both.                  	|
|      *THING*     	| [Notice the italic] Replace *THING* with whatever is appropriate. 	|


```
$ help cd
```
-- Some commands does not have mannual pages that time we can use help to see it's descriptive information.
