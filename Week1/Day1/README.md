# Week1 - Day 1

## Problems

# Problem 1

void fun(int w, int x){
    int y =0;
    if((x%w==0) || (w%x==0)){
        y += 1
    }else{
        y += 10
    }
    print(y)
}

fun(40,4)


### options
- 1
- 11
- 10 
- 2

**answer:**  1


# Problem 2

Total no of times the loop runs

int a =1;
while(a<5){
    a += 2
}
print(a)


### options
- 1
- 4
- 2 
- 3

**answer:**  2

> explanation: When while loop is executed 1st time, a is incremented to 3, next time again it enters loop and a is 
incremented to 5. Next time, while loop is not entered. Hence while loop is executed twice.  

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

# Problem 4

int a=3, b=3
a=b
if( 1 ^ 1){
    a=1
}else{
    b=2
}
print(a+b)


### options
- 1
- 16
- 5 
- 6

**answer:**  5

# Problem 5

int fun(a,b){
    int c;
    for(each c from 2 to 4){
        if(a%2 < b%3){
            a=4%3
        }else{
            if(5%3 > b){
                a=b
            }
            b=1
        }
    }
    return a+b
}

fun(7,5)

### options 
- 23
- -2
- 6
- 8


**solution:** 6

> the loop would never go to else block and the final result is a=1 and b=5 => a+b = 1+5 = 6 

# Problem 6

int fun(int a, int b){
    if(a>0){
       return fun(a-2,a+b) + fun(a-3,a+b) + fun(a-4,a+b);
    }else{
        a = b
        b = a
        return a+b
    }
}

fun(4,3)


### options
- 116
- 117
- 114
- 125

**answer:**  116

# Problem 7

int fun(int a, int b){
    a = a+a;
    b = b+b;
    return a+b

}

fun(6,1)


### options
- 23
- 14
- 12
- 16

**answer:**  14

>  a = 6+6 = 12 ; b = 1+1 = 2. Return 12+2 that is 14. Hence ans is 14.  

### Problem 8

int a=2,b=4,c-2
if(b-a){
    a = a^b
    a=c
    if(b){
        a=a^b
    }
    b=b-1
}
if(c){
    a=b
}

print(a+b+c)

### options 
 - 13
 - 12
 - 30
 - 9

 **solution:** 12
