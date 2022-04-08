####쉘 스크립트
```
$ gedit ex01.sh     
```
'''''''''ex01.sh'''''''''     
-#!/bin/sh   
echo "me home:" $HOME  
'''''''''ex01.sh''''''''' 

```
$ sh ex01.sh (쉘로 실행하기)      
me home: /home/user1

$ ./ex01.sh (권한이 없을시 chmod로 실행 권한준 뒤 실행)    
me home: /home/user1
```

```
$ gedit ex01.sh
```

'''''''''ex01.sh'''''''''     
-#!/bin/sh   
echo "me home:" $HOME  
exit 1  
'''''''''ex01.sh''''''''' 

```
$ ./ex01.sh > result.txt 1> result2.txt
```

출력 방향을 바꾸는데 예외가 발생하면 exit 번호에 따라 출력을 바꿈

'''''''''result2.txt'''''''''   
me home: /home/user1   
'''''''''result2.txt'''''''''
