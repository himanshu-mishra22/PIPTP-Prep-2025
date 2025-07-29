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
