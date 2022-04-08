####반복문

for

```
$ gedit ex09.sh
```

<pre>

'''''''''ex09.sh'''''''''   
 #!/bin/sh  
 for fname in $(ls ex*.sh)   
 do   
	echo "-----------"   
	ls -l $fname   
 done   
'''''''''ex09.sh'''''''''
</pre>

```
$ ./ex09.sh
~ ex01.sh
~ ex02.sh
~ ex03.sh
~ ex04.sh
~ ex05.sh
~ ex06.sh
```

while

```
while [  ]
do
~~
done