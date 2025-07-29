# Problem 3

int fun(int a, int b){
   if(a && b && a+b > 0){
     return a + fun(a-2,b-2)+b
   }

   return a ^ b
}

fun(8,8)


### options
- 39
- 46
- 48 
- 40

**answer:**  40

> recursive function at (0,0) would be a ^ b = 0 which will add to the previous call stack having value of a + **fun(a-2,b-2) will be 0** + b => 4 and so on...

