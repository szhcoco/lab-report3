## Commands I choose: ```grep```
The first interesting command option for ```grep``` is ```ls |grep ```. The command is used to find all of the files in the directory that contain the string in its name. 
### Example1:
```
# code block
zhanghui@s-MacBook-Pro berlitz2 % ls |grep Algarve
Algarve-History.txt
Algarve-Intro.txt
Algarve-WhatToDo.txt
Algarve-WhereToGo.txt
```
I change the directory in to berlitz2 and use ```ls |grep Algarve ```to find all the text file that has contains ```Algarve ```in its name. It can be useful if you want to find the txt files while forgetting about its full name. 

### Example2:
```
# code block
zhanghui@s-MacBook-Pro berlitz2 % ls |grep ToDo
Algarve-WhatToDo.txt
Amsterdam-WhatToDo.txt
Athens-WhatToDo.txt
Bahamas-WhatToDo.txt
Bali-WhatToDo.txt
Barcelona-WhatToDo.txt
Beijing-WhatToDo.txt
Berlin-WhatToDo.txt
Bermuda-WhatToDo.txt
Budapest-WhatToDo.txt
California-WhatToDo.txt
CanaryIslands-WhatToDo.txt
Cancun-WhatToDo.txt
China-WhatToDo.txt
Costa-WhatToDo.txt
CostaBlanca-WhatToDo.txt
Crete-WhatToDo.txt
Cuba-WhatToDo.txt
Nepal-WhatToDo.txt
Paris-WhatToDo.txt
Poland-WhatToDo.txt
Portugal-WhatToDo.txt
PuertoRico-WhatToDo.txt
Vallarta-WhatToDo.txt
```
In this example, I found all of the text file in the directy ```berlitz2 ``` that contains the ```ToDo ```. It would take lots of time if we manually look through the files in the directory to look for certain file with ```ToDo ```in its name, while this command shows us the output in seconds. 

Another command I found interesting is the ```ls |grep -v```. This command can filter out any txt file whose name contains the given string
### Example1:
```
# code block
zhanghui@s-MacBook-Pro berlitz2 % ls |grep -v To  
Algarve-History.txt
Algarve-Intro.txt
Amsterdam-History.txt
Amsterdam-Intro.txt
Athens-History.txt
Athens-Intro.txt
Bahamas-History.txt
Bahamas-Intro.txt
Bali-History.txt
Barcelona-History.txt
Beijing-History.txt
Berlin-History.txt
Bermuda-history.txt
Budapest-History.txt
Budapest-WhereoGo.txt
California-History.txt
Canada-History.txt
CanaryIslands-History.txt
Cancun-History.txt
China-History.txt
Costa-History.txt
CostaBlanca-History.txt
Crete-History.txt
Cuba-History.txt
Nepal-History.txt
NewOrleans-History.txt
Poland-History.txt
Portugal-History.txt
PuertoRico-History.txt
Vallarta-History.txt
```
In this example, I filtered out any file in ```berlitz2 ```whose name contains the string ```To ```. As a result, the output is the list of file whose name does not contain ```To ```, which saves us a lot of time if we want some files with specific names. 

### Example 2
```
# code block
zhanghui@s-MacBook-Pro OUP % ls  |grep -v ch 
Abernathy
Berk
Castro
Kauffman
Rybczynski
```
In this example, I searched all directories in the directory ```OUP ``` whose name does not contain ```ch ```. With```-v ```, I am able to go through every directory in the ```OUP ``` and find all directories that meet certain requirement. 
