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

