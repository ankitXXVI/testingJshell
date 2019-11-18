# Repository for testing jshel

First commit errors:

jshell>  

jshell> b = n;  
|  Error:  
|  incompatible types: possible lossy conversion from int to byte  
|  b = n;  
|      ^  

jshell> C = n;  
|  Error:  
|  cannot find symbol  
|    symbol:   variable C  
|  C = n;  
|  ^  

### After errors fixed:
int n = 68;  
byte b = 127;  
char c = 'B';  
b = (byte)n;  
c = (char)n;  
b ==> 68  
c ==> 'D'  
