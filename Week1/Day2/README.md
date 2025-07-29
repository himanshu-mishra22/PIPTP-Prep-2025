# Week1 - Day 2

## Problems

### Problem 1
   > int a=2,b=6,c=8
    a=(18+9)+c
    if((c+b)>(a-c)){
        a=b+c
        b=b+b
    }

    print(a+b+c)

 ### options
 A. 23
 B. 41
 C. 48
 D. 58

 **solution :** B

 - In the Line (Statement) no. 3, it is updating the value of variable ‘a’ from 2 to (10+9)+c =>19+8=> 27
 In the Line (Statement) no. 4, it is a conditional statement and evaluates expression with the updated value of
 variable a, because order of statement matters. Since (c+b means 8+6 =14) is not greater than (a-c means 27-8=19),
 the ‘if’ body will not be executed. That’s why it will come directly at statement 8 and will display the sum of a+b+c,
 which is 27+6+8=41, which means option B will be the correct answer from the above given options.

### Problem 2

> int fun(int a, int b, int c){
    b=7+a
    a=(a+c)+a
    b=(b+b)+c
    c=1+b
    return a+b+c
}
fun(0,2,10)

 ### options   
 A. 59
 B. 68
 C. 70
 D. 39

 **solution :** A

 - Initial values will be updated as per the order of statements. Like in Line (statement) no. 3: variable ‘b’
 will be updated with a value of (7+a) which means 7+0=7. Then, in line 4, variable ‘a’ will be updated with value
 (a+c)+a which is (0+10)+0=10. Now, in line 5 ‘b’ will be reupdated with (b+b)+c. Keep remember “Precedence of
 Operators” while assigning the values in ‘b’. First it will execute parenthesis () and will retrieve the current value of b
 which has updated from line 3 then it will add with value of ‘c’. After execution of line 5 variable ‘b’ will be updated
 with value (7+7)+10=24. Then, in line 6, the value of variable ‘c’ will be updated with 1+b. Last value of b is 24 so
 variable ‘c’ will be updated with 1+24=25. Now, from line 7 updated values of variable a, b and c will be added
 together and return from the function. So the final (return) value will be a+b+c => 10+24+25=59. So the final
 answer will be option A, 59.


## Problem 3

> int pp=0,qq=6,rr=7
pp=rr+pp
pp=(rr&4)^rr
if((qq&pp&rr)<(rr&qq)){
    if((qq^pp)<(rr+qq)){
        rr=(3+1)^pp
    }
}

print(pp+qq+rr)

 ### options   

 A. 29
 B. 18
 C. 10
 D. 16

 **solution :** D

 - In line 3, variable pp will be updated with value 7+0=7. In line 4, variable pp will be reupdated; first
 parenthesis will be resolved/evaluated then value will be evaluated with variable rr with XOR operator, means
 (7&4)^7=4^7=3. In line 5, ‘if’ condition will be evaluated, (6&3&7) < (7&6) => 2<6, since the condition is True, it will
 go inside, and then from line 6, it will evaluate the next condition in inner ‘if’, (6^3)<(7+6) => 5<13, since the
 condition is True, line 7 will be executed. In line 7, variable rr will be updated with value (4^3)=7. Now statement 10
 will be executed with an updated value of variables pp, qq and rr, which means 3+6+7=16. So the final output will
 be 16, which is option D.


## Problemm 4
> int p=9, q=6,r=10
if((q ^ p ^ r) > (r ^ q)){
    r=(11&12)+q
}
if((q ^ 6 ^ 8)>(p ^ 4)){
    p=(r+3)&r
}

print(p+q+r)

### options   

 A. 20
 B. 27
 C. 25
 D. 36

 **solution :** C

 - In line 3, ‘if’ will be checked for the condition: (6 ^9 ^ 10) > (10 ^ 6) => 5 > 12 => False. Since the
 condition is false, line 4 will be skipped, as line 4 is part of ‘if’. Then it will come on line 6 and will check the next ‘if’
 condition, which is: (6 ^ 6 ^ 8) > (9 ^ 4) => 8 > 13 => False. Since this ‘if’ condition is false, it will skip line 7. Then it will
 come on line 9, and will add all three variables: 9+6+10=25, which is option C

## Problem 5
> int p=9,q=6,r=10
if((q ^ p ^ r)> (r ^ q)){
    r=(qq&12)+q
}
if((q ^ 6 ^ 8) > (q ^ 4)){
    p=(r+3)&r
}
print(p+q+r)


### options

 A. 20
 B. 27
 C. 25
 D. 36

 -  In line 3, ‘if’ will be checked for the condition: (6 ^ 9 ^ 10) > (10 ^ 6) => 5 > 12 => False. Since the
 condition is false, line 4 will be skipped, as line 4 is part of ‘if’. Then it will come on line 6 and will check the next ‘if’
 condition, which is: (6 ^ 6 ^ 8) > (9 ^ 4) => 8 > 13 => False. Since this ‘if’ condition is false, it will skip line 7. Then it will
 come on line 9, and will add all three variables: 9+6+10=25, which is option C

 
