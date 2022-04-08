####출력
```
$ echo 'abc$HOME'
abc$HOME

$ echo "abc$HOME"
abc/home/user1
```

```
$ nano ex03.sh
```

<pre>

'''''''''ex03.sh'''''''''    
 #!/bin/sh   
var1="hello world"   
echo $var1   
echo "$var1"   
echo '$var1'   
echo \$var1   
echo input:   
read var1   
echo 'var=' $var1   
'''''''''ex03.sh'''''''''
</pre> 

```
hello world
hello world
$var1
$var1
input:
shell
var=shell
$ sh ex03.sh
```

```
$ gedit ex04.sh
```

<pre>

'''''''''ex04.sh'''''''''   
 #!/bin/sh   
num1=100   
num2=10   
num3=num1+num2   
echo $num1   
echo $num2   
echo $num3   
echo `expr $num1 + $num2`   
'''''''''ex04.sh'''''''''
</pre>

```
$ sh ex04.sh
100
10
num1+num2
110
```

<pre>

'''''''''ex04.sh'''''''''   
 #!/bin/sh   
num1=100   
num2=10   
num3=num1+num2   
echo $num1   
echo $num2   
echo $num3   
echo `expr \( $num1 + $num \) \* 2'   
'''''''''ex04.sh'''''''''
</pre>

```
$ sh ex04.sh
100
10
num1+num2
220
```

```
$ gedit ex05.sh
```

<pre>

'''''''''ex05.sh'''''''''   
 #!/bin/sh   
echo "1 = <$0>" 
echo "2 = <$1>" 
echo "3 = <$2>" 
echo "all = <$*>" 
'''''''''ex05.sh'''''''''
</pre>

```
sh ex05.sh aaa bbb ccc
1 = <ex05.sh>
2 = <aaa>
3 = <bbb>
all = <aaa bbb ccc>
```



