####if
* 괄호 안 양쪽 공백필수   
if [  ] : false    
if [ 1 ] : true 

```
$ gedit ex06.sh
```

<pre> 

'''''''''ex06.sh'''''''''
 #!/bin/sh 
echo "start..."   
if [ 1 ]

then   
	echo "result:true"   

fi   
echo "end..."  
'''''''''ex06.sh'''''''''
</pre>

```
$ sh ex06.sh
start...
result: true
end...
```
