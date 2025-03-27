# Polonium Coding Style    

## 1. Casing types and examples of them:   
 - Pascal Case: `KiKernelStartup`, `ShowWindow`, `PoAddObject`
 - Macro Case: `INIT_EXECUTABLE_NAME`
 - Uppercase: `GDTENTRY`, `CPU`
 - Snake Case: `radiom_cpp`
 - Camel Case: `basicVariable`

## 2. C Function naming:
2.1. Functions should be called using pascal case    
2.2. Functions in RTL (Runtime Library) should be prefixed with Rtl namespace    
2.3. Functions in kernel should be prefixed with kernel namespace that they belong.      
2.4. If function is internal but you think it would be useful in another place you should:     
     - If function is prefixed with namespace you should replace last letter of the namespace prefix with small i    
     - Else you should add I (Big one) on the start of Function name     
2.5. If function is private or static:    
     - If function is prefixed with namespace you should replace add letter to the namespace prefix with small p     
     - Else you should add P (Big one) on the start of Function name    
2.6. Arguments should be called using pascal case       

## 3. C Variables naming       
3.1. Public global variables should be named using pascal case and if it is in kernel it should be prefixed with namespace     
3.2. Private global variables should be named using pascal case with p prefix (you shouldnt add namespace prefix)      
3.3. Local variables in functions should be called using camel case     

## 4. Struct naming        
4.1. Struct should be defined using typedefs     
4.2. Appropriate casing for structs are Uppercase      
4.3. You should define members using pascal case       
4.4. You should prefix private members with p (small one)         